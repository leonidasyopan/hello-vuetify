<template lang="pug">
  v-app
    v-content
      router-view
</template>

<script>
export default {
  name: "App",

  components: {},

  data: () => ({
    bars: [
      { class: "" },
      { class: "", dark: true },
      { class: "primary", dark: true },
      { class: "elevation-0" },
    ],
  }),
};
</script>
