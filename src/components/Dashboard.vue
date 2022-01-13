<template>
  <div class="dashboard">
    <div class="flex-space">
    <HomeBase/>
    <div class="cards">
      <IntroCard/>
      <div class="flex">
        <EmptyCard/>
        <ToDoCard :todos="todoData" />
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
import axios from 'axios'


@Options({
  data() {
    return {
      todoData: null
    }
  },
  components: {
    HomeBase,
    IntroCard,
    EmptyCard,
    ToDoCard,
  },
  mounted () {
    /* Get data for ToDo list component */
    axios
      .get('https://jsonplaceholder.typicode.com/todos')
      .then(response => (this.todoData = response.data))
      .catch(error => console.log(error))
  }
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
</style>
