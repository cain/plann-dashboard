<template>
  <div class="top-banner">
    <img class="logo-img" alt="Vue logo" src="../assets/images/plann-logo.png">
  </div>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component';

export default class TopBanner extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .top-banner {
    background-color: white;
    height: 60px;
  }

  .logo-img {
    cursor: pointer;
  }
</style>
