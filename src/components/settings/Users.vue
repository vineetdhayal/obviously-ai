<script setup lang="ts">
import BoxUser from "./BoxUser.vue";
import UserDelete from "./UserDelete.vue";

</script>
<template>
  <div class="flex direction border profileGap">
    <div class="bold">User Seats</div>
    <div>Invite another user from your company to Obviously AI.</div>
    <div class="flexBox">
      <BoxUser type="Name" value="The Rock" />
      <BoxUser type="Email" value="dwayne.rock@microsoft.com" />
      <div class="plus">+</div>
    </div>
    <div>Existing Users</div>
    <div class="flexUser">
      <UserDelete
        type="Monica Greenleaf"
        value="monica.greenleaf@microsoft.com"
      />
      <UserDelete
        type="Monica Greenleaf"
        value="monica.greenleaf@microsoft.com"
      />
      <UserDelete
        type="Monica Greenleaf"
        value="monica.greenleaf@microsoft.com"
      />
      <UserDelete
        type="Monica Greenleaf"
        value="monica.greenleaf@microsoft.com"
      />
    </div>
  </div>
</template>

<style scoped>
@import "./user.css";
</style>
