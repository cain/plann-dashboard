<template>
  <div class="card empty-card">

  </div>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component';

export default class EmptyCard extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

 /* Override plann-theme.css card */
  .card {
    width: 70%;
    height: 120px;
  }
</style>
