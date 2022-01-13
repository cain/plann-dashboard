<template>
  <div class="card">
    <span class="dark-blue-text intro-text-small">Hi </span> 
    <span class="light-blue-text intro-text-small">Christy,</span>
    <div class="dark-blue-text intro-text-large">Welcome back 👋</div>
  </div>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component';

export default class IntroCard extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .intro-text-small {
    font-size: 32px;
  }

  .intro-text-large {
    font-size: 48px;
  }

  .card {
    height: 120px;
  }
</style>
