<template>
  <div class="top-banner">
    <img alt="Vue logo" src="../assets/Plann_logo.png">

    <button class="">
    <span>
      Home Base
    </span>
  </button>
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

  button {
    border-radius: 10px;
    padding: 24px 60px;
    background-color: #81C4EE;
    border: none;
    text-transform: uppercase;
    cursor: pointer;
    background-color: #fff;
  border-color: #fafbff;
  border-width: 1px;
  color: #293147;
  cursor: pointer;
  justify-content: center;
  padding-bottom: calc(.5em - 1px);
  padding-left: 1.75em;
  padding-right: 1.75em;
  padding-top: calc(.5em - 1px);
  text-align: center;
  white-space: nowrap;
}
</style>
