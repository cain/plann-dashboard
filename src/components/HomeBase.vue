<template>
  <div class="home-base-button">
    <button class="button-home">
      <span class="inner-text upper-case-text">
      Home Base
      </span>
  </button>
  </div>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component';

export default class HomeBase extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .home-base-button {
    margin: 10px;
    margin-right: 50px;
  }

  .button-home {
    color: white;
    border-radius: 10px;
    padding: 1.5em 4em;
    background-color: #81C4EE;
    border:none;
    cursor: pointer;
    text-align: center;
    white-space: nowrap;
    transition: all 0.2s;
}

  .button-home .inner-text {
    font-weight: 700;
    font-size: 1.3em;
  }

  button:hover {
    background-color: #67b8eb;
}
</style>
