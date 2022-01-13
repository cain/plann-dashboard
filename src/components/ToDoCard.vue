<template>
<div class="card todo-list">
    <div class="todo-title dark-blue-text upper-case-text">
        Your to-dos for today
    </div>
    <div v-for="todo in todos" :key="todo.id">
        <div v-if="todo.id <= 5">
            <div v-if="todo.completed">
                <div class="todo-item todo-item-complete">
                    <div class="flex">
                        <img class="todo-img" src="../assets/images/presentation-icon.svg">
                        <span class="todo-item-title" v-text="todo.title"></span>
                    </div>
                    <div class="todo-item-description">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vehicula est lucas.</div>
                    <div class="flex">
                        <img class="todo-img" src="../assets/images/user-icon.svg">
                        <span class="todo-item-user">User Name</span>
                    </div>
                </div>
            </div>
            <div v-else>
                <div class="todo-item todo-item-incomplete">
                    <div class="flex">
                        <img class="todo-img" src="../assets/images/mail-icon.svg">
                        <span class="todo-item-title" v-text="todo.title"></span>
                    </div>
                    <div class="todo-item-description">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis vehicula est lucas.</div>
                    <div class="flex">
                        <img class="todo-img" src="../assets/images/user-icon.svg">
                        <span class="todo-item-user">User Name</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="todo-see-all upper-case-text">See All</div>
</div>
</template>

<script lang="ts">
import {
    Options,
    Vue
} from 'vue-class-component';

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
    todos!: Array < ToDoInterface >
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
/* Override plann-theme.css card */
.card {
    height: 500px;
    width: 30%;
}

@import '../assets/styles/todo-style.css';
</style>
