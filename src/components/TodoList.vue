<template>
  <div>
    <h1 class="title is-1">Todo List with VueJS</h1>
    <TodoInputText />
    <TodoListItem :todos="todos" />
  </div>
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";
import TodoListItem from "@/components/TodoListItem.vue";

export default {
  components: {
    TodoInputText,
    TodoListItem
  },

  data() {
    return {
      todos: ["Task one", "Task two", "Task three"]
    };
  }
};
</script>

<style>
</style>