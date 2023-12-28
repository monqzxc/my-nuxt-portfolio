<script setup></script>

<template>
  <div class="w-full flex items-center mt-6 p-4 px-10">
    <div class="flex flex-auto items-center">
      <h1 class="text-6xl font-bold text-primary-500">Projects</h1>
    </div>
  </div>

  <section class="flex flex-col gap-10 ml-10">
    <TransitionGroup name="fade" appear>
      <div
        v-for="(project, index) in projects"
        :key="project"
        v-bind:style="[
          index < 9
            ? { 'transition-delay': 0 }
            : {
                'transition-delay': `${(index % 10) * 100}ms`,
              },
        ]"
      >
        <ProjectTile
          :title="project.title"
          :image="project.image"
          :content="project.content"
          :url="project.url"
        />
      </div>
    </TransitionGroup>
  </section>
</template>
<script>
import ProjectTile from "~/components/ProjectTile.vue";
import {
  survey,
  job_opening,
  employee_profile,
  leaves,
} from "~/public/references";

export default {
  components: {
    ProjectTile,
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Survey Form",
          image: survey,
          content:
            "One of the modules and part of the HRIS is this survey form. It is used when gathering information from the inquiry of the clients.",
          url: "https://survey.tesda.gov.ph/survey-form/co",
        },
        {
          id: 2,
          title: "Job Application Page",
          image: job_opening,
          content:
            "An online job application for TESDA. It also has an application profile where uploading of requirements, and the status of application can be seen. Tho it's not publicized and still in staging.",
          url: "",
        },
        {
          id: 3,
          title: "Employee Profile Module",
          image: employee_profile,
          content:
            "An internal profile page for the employees. It contains their employment profile, and all of the contents of Personal Data Sheet. Can also Generate Personal Data Sheet PDF.",
          url: "",
        },
        {
          id: 4,
          title: "Leave Administration Module",
          image: leaves,
          content:
            "It's also a part of HRIS, the Leaves Administration module. Where applying, viewing, approving, and disapproving of Leaves and Official Businesses (OB) are managed.",
          url: "",
        },
      ],
    };
  },
};
</script>

<style scoped>
.fade-move,
.fade-enter-active,
.fade-leave-active {
  transition: all 0.8s cubic-bezier(0.55, 0, 0.1, 1);
  z-index: 0;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
  transform: scaleY(0.01) translate(30px, 0);
}

.fade-leave-active {
  position: absolute;
}
</style>
