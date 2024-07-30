<script setup lang="ts">
import { ref } from "vue";
import BoxNormal from "./BoxNormal.vue";
import BoxEqual from './BoxEqual.vue';
import BoxSmall from "./BoxSmall.vue";
</script>

<template>
  <div class="main flex direction profileGap">
    <img class="rightImage" src="../../assets/group2.svg" />
    <div class="flex direction">
      <div class="firstFont">All datasets</div>
      <div class="firstFont">to your Obviously account</div>
      <div class="secondFont">
        Add dataset for making predictions. We don’t and will never store your
        data.
      </div>
    </div>
    <div>Upload a file</div>
    <button>Upload a csv</button>
    <div class="flex">
      <div class="left-line"></div>
      OR
      <div class="right-line"></div>
    </div>
    <div>
      <div>Connect a database</div>
      <div>
        In order to ensure Obviously AI has access to your database, please
        whitelist our IP address 104.198.187.43 on your database firewall.
      </div>
    </div>
    <div class="flex profileGap">
      <img src="../../assets/sql.png" class="myImage" />
      <img src="../../assets/sql.png" class="myImage green" />
    </div>
    <div class="flex boxGap">
      <BoxSmall type="Display Name" value="monica.greenleaf@factset.com" />
      <BoxNormal type="Description" value="monica greenleaf" />
    </div>
    <div class="flex boxGap">
      <BoxNormal type="Description" value="monica greenleaf" />
      <BoxSmall type="Display Name" value="monica.greenleaf@factset.com" />
    </div>
    <div class="flex boxGap">
      <BoxEqual type="Display Name" value="monica.greenleaf@factset.com" />
      <BoxEqual type="Display Name" value="monica.greenleaf@factset.com" />
      <BoxEqual type="Display Name" value="monica.greenleaf@factset.com" />
    </div>
    <button class="my-button">Add This Database</button>
  </div>
</template>

<style scoped>
@import "./right-section.css";
</style>
