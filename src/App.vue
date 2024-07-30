<script setup lang="ts">
import SettingsPage from "./components/settings/SettingsPage.vue";
import DataBase from "./components/data-base/DataBase.vue";
import { computed, ref } from "vue";

const routes: any = { "/": SettingsPage, "/database": DataBase };

const currentPath = ref(window.location.pathname);
console.log(currentPath);

window.addEventListener("hashchange", () => {
  currentPath.value = window.location.pathname;
  console.log(currentPath.value);
});

const currentView = computed(() => {
  return routes[currentPath.value || "/" as any];
});
</script>

<template>
  <component :is="currentView" />
</template>

<style scoped>
</style>
