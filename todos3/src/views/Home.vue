<template>
  <div class="home">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from "../components/Todos.vue";
export default {
  name: "home",
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Todo One",
          completed: false
        },
        {
          id: 2,
          title: "Todo Two",
          completed: true
        },
        {
          id: 3,
          title: "Todo Three",
          completed: false
        }
      ]
    };
  }
};
</script>

<style scoped>
* {
  border-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: Helvetica, Arial, sans-serif;
  line-height: 1.4;
}
</style>
