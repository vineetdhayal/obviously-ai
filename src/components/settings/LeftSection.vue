<script setup lang="ts">
import { ref } from "vue";
</script>

<template>
  <div class="flex logo">
    <img src="../../assets/logo.png" class="img" />
    <input type="radio" />
  </div>
  <div class="background flex profileGap">
    <img src="../../assets/profile.png" class="profile" />
    <div>
      <div>Monica Greenleaf</div>
      <div>Microsoft</div>
    </div>
  </div>
  <div class="flex direction profileGap">
    <div>Explore</div>
    <div>Definitions</div>
    <div>Settings</div>
    <div>Help</div>
  </div>
  <div class="break-line"></div>
  <div class="flex logo">
    <div>My Predictions</div>
    <div class="plus-button"></div>
  </div>
  <div class="flex direction profileGap">
    <div class="radio-gap flex">
      <input type="radio" class="radio-button" />
      <label>MoM user churn for Q3</label>
    </div>
    <div class="radio-gap flex">
      <input type="radio" class="radio-button" />
      <label>Merch sales for Jan</label>
    </div>
    <div class="radio-gap flex">
      <input type="radio" class="radio-button" />
      <label>State-wise donor prediction</label>
    </div>
  </div>
  <div class="font">Show All</div>
  <div class="break-line"></div>
  <div class="flex logo">
    <div>My DataSets</div>
    <div class="plus-button"></div>
  </div>
  <div class="flex direction profileGap">
    <div class="radio-gap flex">
      <input type="radio" class="radio-button" />
      <label>Twitch Data</label>
    </div>
    <div class="radio-gap flex">
      <input type="radio" class="radio-button" />
      <label>Slobs User Data</label>
    </div>
    <div class="radio-gap flex">
      <input type="radio" class="radio-button" />
      <label>External csv file</label>
    </div>
  </div>
  <div class="font">Show All</div>
</template>

<style scoped>
@import "./left-section.css";
</style>
