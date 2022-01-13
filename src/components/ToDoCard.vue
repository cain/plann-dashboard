<template>
  <div class="card">
    <div class="todo-title dark-blue-text upper-case-text">
      Your to-dos for today
    </div>
  </div>
</template>

<script lang="ts">
import { Vue } from 'vue-class-component';

export default class ToDoCard extends Vue {
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
