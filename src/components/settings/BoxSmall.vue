<script setup lang="ts">
defineProps<{ type: string, value: string }>();
</script>
<template>
  <div class="specsSmall flex direction">
    <div class="bold">{{ type }}</div>
    <div>{{ value }}</div>
  </div>
</template>

<style scoped>
@import "./box-normal.css";
</style>
