<template>
  <div class="p-4 flex gap-2 flex-col">
    <h1 class="font-bold text-lg">{{ title }}</h1>
    <img :src="image" style="width: 100vh; height: 50vh" />

    <p class="rounded-lg p-2 shadow-lg">
      {{ content }}
    </p>
    <a
      v-if="url != ''"
      class="font-bold text-indigo-900"
      target="_blank"
      :href="url"
      >Visit Site</a
    >
    <p v-else class="italic text-xs text-red-400">
      Viewable page is not available due to internal use or not yet publicized
    </p>
  </div>
</template>
<script>
export default {
  props: {
    title: String,
    image: String,
    content: String,
    url: String,
  },
};
</script>
