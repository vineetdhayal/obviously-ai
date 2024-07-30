<script setup lang="ts">
defineProps<{ type: string; value: string }>();
</script>
<template>
  <div class="specsUser flex spacing">
    <div class="flex direction">
      <div class="bold">{{ type }}</div>
      <div class="font-small">{{ value }}</div>
    </div>
    <div class="price">➕</div>
    <div class="price">❌</div>
  </div>
</template>

<style scoped>
@import "./box-normal.css";
</style>
