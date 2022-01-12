<template>
  <div class="dashboard">
    <HomeBase/>
    <IntroCard/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HomeBase from '../components/HomeBase.vue';
import IntroCard from '../components/IntroCard.vue';

@Options({
  components: {
    HomeBase,
    IntroCard,
  },
})
export default class Dashboard extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .dashboard {
    margin: 40px;
    display: flex;
    justify-content: space-between;
  }
</style>
