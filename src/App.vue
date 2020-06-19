<template lang="pug">
  v-row
    v-col(
      v-for="(bar, i) in bars"
      :key="i"
      cols="12"
      sm="12"
      md="6"
      class="my-4"
    )
    
      v-card(color="grey lighten-4" flat height="200px")
        v-toolbar(:color="bar.class" :dark="bar.dark")
          v-app-bar-nav-icon
          v-toolbar-title
          v-spacer
          v-btn icon
            v-icon
          
          v-btn icon
            v-icon
          
          v-btn icon
            v-icon
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
