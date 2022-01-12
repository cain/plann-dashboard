<template>
  <div class="top-banner">
    <img alt="Vue logo" src="../assets/Plann_logo.png">
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    msg: String
  }
})
export default class TopBanner extends Vue {
  msg!: string
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .top-banner {
    background-color: white;
    height: 60px;
  }
</style>
