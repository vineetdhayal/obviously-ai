<script setup lang="ts">
import LeftSection from "./LeftSection.vue";
import RightSection from "./RightSection.vue";

defineProps<{ type: string; value: string }>();
</script>
<template>
  <div class="flex">
    <div class="flex-left">
      <LeftSection />
    </div>
    <div class="flex-right">
      <RightSection />
    </div>
  </div>
</template>

<style scoped>
.flex {
  display: flex;
  gap: 20px;
  height: 100%;
}

.flex-left {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  gap: 50px;
  padding: 15px;
  background-color: darkgray;
}

.flex-right {
  flex-grow: 4;
  max-width: 1500px;
}
</style>
