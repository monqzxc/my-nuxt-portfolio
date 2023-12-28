<script setup></script>

<template>
  <div class="w-full flex items-center mt-6 p-4 px-10">
    <div class="flex flex-auto items-center">
      <h1 class="text-6xl font-bold text-primary-500">Achievements</h1>
    </div>
  </div>

  <section class="flex flex-col gap-6 p-10">
    <div v-for="a in achievements" :key="a.id" class="p-2 shadow-lg rounded-lg">
      <div>
        <div class="flex flex-row gap-2 items-center">
          <div><img src="/bullet.png" style="width: 15px; height: 15px" /></div>
          <div class="font-bold text-yellow-500 text-lg">
            {{ a.title }}
          </div>
        </div>
        <div class="text-sm ml-6">{{ a.date }}</div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      achievements: [
        {
          title:
            "Competitor for IT Software Solutions for Business in WorldSkills Kazan, Russia 2019",
          date: "August 2019",
        },
        {
          title:
            "Medallion for Excellence in IT Software Solutions for Business in WorldSkills ASEAN Bangkok 2018",
          date: "September 2018",
        },
        {
          title:
            "Silver Medalist in IT Software Solutions for Business in Zonal Skills Competition 2017",
          date: "December 2017",
        },
        {
          title:
            "Gold Medalist in IT Software Solutions for Business in Regional Skills Competition 2017",
          date: "October 2017",
        },
        {
          title:
            "Gold Medalist in IT Software Solutions for Business in Pampanga Skills Competition 2017",
          date: "August 2017",
        },
      ],
    };
  },
};
</script>
