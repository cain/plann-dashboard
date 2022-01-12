<template>
  <div class="app">
    <TopBanner />
    <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HelloWorld from './components/HelloWorld.vue';
import TopBanner from './components/TopBanner.vue';

@Options({
  components: {
    HelloWorld,
    TopBanner,
  },
})
export default class App extends Vue {}
</script>

<style>
.app {
  /* Since Proxima Nova is a paid font I used googles free alternative */
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body {
  margin: 0px;
  background-color: #F5F8FF;
}
</style>
