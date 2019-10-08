<template>
  <div id="app" class="container">
    <TodoList />
  </div>
</template>

<script>
import TodoList from "@/components/TodoList.vue";

export default {
  name: "app",
  components: {
    TodoList
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  font-size: 10px;
}

.container {
  display: grid;
  align-items: center;
  justify-items: center;
  margin-top: 2rem;
}
</style>
