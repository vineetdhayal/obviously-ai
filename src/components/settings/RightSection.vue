<script setup lang="ts">
import { ref } from "vue";
import BoxNormal from "./BoxNormal.vue";
import BoxSmall from "./BoxSmall.vue";
import MemberShip from './MemberShip.vue';
import Users from './Users.vue';
</script>

<template>
  <div class="main flex direction profileGap">
    <div class="flex direction boxGap">
      <div class="firstFont">All your</div>
      <div class="firstFont">Settings in one place</div>
      <div class="secondFont">manage account details, billing and users</div>
    </div>
    <div class="flex width boxGap">
      <BoxNormal type="Name" value="Monica Greenleaf" />
      <BoxNormal type="Company" value="Microsoft Inc." />
      <BoxNormal type="Email" value="monica.greenleaf@microft.com" />
      <BoxNormal type="Current Password" value="*********" />
      <BoxNormal type="New Password" value="**********" />
      <BoxNormal type="Repeat Password" value="*********" />
      <BoxNormal type="Card Number" value="1234-3455-5677-5677" />
      <BoxNormal type="Expiration" value="03/11" />
      <BoxSmall type="CVV" value="240" />
      <BoxSmall type="ZIP" value="01002" />
    </div>
    <div class="flex boxGap">
      <MemberShip class="membership" />
      <Users class="users"/>
    </div>
    <button class="my-button">Update All Settings</button>
  </div>
</template>

<style scoped>
@import "./right-section.css";
</style>
