<template>
  <div class="card">
    <div class="todo-title dark-blue-text upper-case-text">
      Your to-dos for today
    </div>
  <div v-for="todo in todos" :key="todo.id">
    <div v-if="todo.id <= 5">
      <div v-if="todo.completed">
        <div v-text="todo.title" class="to-do-item-completed">
          <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vehicula est lucas.</div>
        </div>
      </div>
      <div v-else> 
        <div v-text="todo.title" class="to-do-item">
          <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vehicula est lucas.</div>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

    export interface ToDoInterface {
        userId: number;
        id: number;
        title: string;
        completed: boolean;
    }

@Options({
  props: {
    todos: Array
  }
})
export default class HelloWorld extends Vue {
  todos!: Array<ToDoInterface>
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.todo-title {
  font-size: 22px;
  font-weight: 700;
}
  .card {
    height: 500px;
    width: 30%;
  }
</style>
