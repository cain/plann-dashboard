<template>
  <div class="home-base-button">
    <button class="button-home">
      <span class="inner-text">
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
export default class HomeBase extends Vue {
  msg!: string
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .button-home {
    color: white;
    border-radius: 10px;
    padding: 1.5em 4em;
    background-color: #81C4EE;
    border:none;
    outline: none;
    cursor: pointer;
    text-align: center;
    white-space: nowrap;
    transition: all 0.2s;
}

  .button-home .inner-text {
    font-weight: 700;
    font-size: 1.3em;
    text-transform: uppercase;
  }

  button:hover {
    background-color: #67b8eb;
    outline: 0.18em solid #67b8eb8e;
}
</style>
