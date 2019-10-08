<template>
  <div>
    <h1 class="title is-1">Todo List with VueJS</h1>
    <TodoInputText v-model="newTodoText" @keydown.enter="addTodo" />
    <TodoListItem :todos="todos" />
  </div>
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";
import TodoListItem from "@/components/TodoListItem.vue";
import { exists } from "fs";

export default {
  components: {
    TodoInputText,
    TodoListItem
  },

  data() {
    return {
      newTodoText: "",
      todos: ["Task one", "Task two", "Task three"]
    };
  },

  methods: {
    addTodo() {
      const trimmedText = this.newTodoText.trim();
      if (trimmedText) {
        this.todos.push(trimmedText);
        this.newTodoText = "";
      }
    }
  }
};
</script>

<style>
</style>