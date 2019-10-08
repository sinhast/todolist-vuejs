<template>
  <div>
    <h1 class="title is-1">Todo List with VueJS</h1>
    <TodoInputText />
  </div>
</template>

<script>
import TodoInputText from "@/components/TodoInputText.vue";

export default {
  components: {
    TodoInputText
  }
};
</script>

<style>
</style>