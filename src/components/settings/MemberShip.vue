<script setup lang="ts">
import { ref } from "vue";
import BoxPrice from "./BoxPrice.vue";

defineProps<{ type: string; value: string }>();
</script>
<template>
  <div class="flex direction profileGap border">
    <div class="bold">MemberShip</div>
    <div>Switch to other plan or cancel membership</div>
    <div>Current Plan</div>
    <BoxPrice
      type="Premium"
      value="Supports 10M rows of data + 5 free user seats"
      price="$799/mo"
    />
    <div>Other Plan</div>
    <BoxPrice
      type="Basic"
      value="Supports 10M rows of data + 5 free user seats"
      price="$299/mo"
    />
    <BoxPrice
      type="Standard"
      value="Supports 10M rows of data + 5 free user seats"
      price="$499/mo"
    />
  </div>
</template>

<style scoped>
@import "./member-ship.css";
</style>
