<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from './components/Todos'

export default {
  name: 'app',
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id:1,
          title: "Todo One",
          completed: true
        },
        {
          id:2,
          title: "Todo Two",
          completed: true
        },
        {
          id:1,
          title: "Todo Three",
          completed: false
        }
      ]
    }
  }
}
</script>

<style>

</style>
