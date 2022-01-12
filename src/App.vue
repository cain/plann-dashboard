<template>
  <div class="app">
    <TopBanner />
    <Dashboard/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Dashboard from './components/Dashboard.vue';
import TopBanner from './components/TopBanner.vue';

@Options({
  components: {
    TopBanner,
    Dashboard,
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

@import './assets/styles/plann-theme.css';
</style>
