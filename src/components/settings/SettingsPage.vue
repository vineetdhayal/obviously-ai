<script setup lang="ts">
import LeftSection from "./LeftSection.vue";
import RightSection from "./RightSection.vue";
</script>

<template>
  <div class="flex">
    <div class="flex-left">
      <LeftSection />
    </div>
    <div class="flex-right backgr">
      <RightSection />
    </div>
  </div>
</template>

<style scoped>
.flex {
  display: flex;
}

.flex-left {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  gap: 20px;
  padding: 15px;
  background-color: darkgray;
}

.flex-right {
  flex-grow: 4;
  max-width: 1500px;
  padding: 30px;
}

label {
  height: 10px;
}

.backgr {
  background-image: url("../../assets/group.svg");
  height: 60%;
  object-fit: cover;
}
</style>
