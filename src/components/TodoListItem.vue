<template>
  <ul>
    <li v-for="todo in todos" :key="todo">{{ todo }}</li>
  </ul>
</template>

<script>
export default {
  props: ["todos"]
};
</script>

<style>
</style>