<script setup lang="ts">
defineProps<{ type: string; value: string; price: string }>();
</script>
<template>
  <div class="specsPrice flex">
    <div class="flex direction">
      <div class="bold">{{ type }}</div>
      <div class="font-small">{{ value }}</div>
    </div>
    <div class="price">{{ price }}</div>
  </div>
</template>

<style scoped>
@import "./box-normal.css";
</style>
