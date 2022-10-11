<template>
  <v-app>
    <AppHeader />
  </v-app>
</template>

<script>
import AppHeader from "./components/task-header.vue";

export default {
  name: "App",

  components: {
    AppHeader,
  },
};
</script>
