<template>
  <div class="dashboard">
    <div class="flex-space">
    <HomeBase/>
    <div class="cards">
      <IntroCard/>
      <div class="flex">
        <EmptyCard/>
        <ToDoCard/>
        </div>
    </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import HomeBase from '../components/HomeBase.vue';
import IntroCard from '../components/IntroCard.vue';
import EmptyCard from '../components/EmptyCard.vue';
import ToDoCard from '../components/ToDoCard.vue';


@Options({
  components: {
    HomeBase,
    IntroCard,
    EmptyCard,
    ToDoCard,
  },
})
export default class Dashboard extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .dashboard {
    margin: 20px;
  }

  .cards {
    width: 100%;
  }

  .flex {
    display: flex;
  }

  .flex-space {
    display: flex;
    justify-content: space-between;
  }
</style>
