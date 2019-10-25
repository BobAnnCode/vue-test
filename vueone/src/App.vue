<template>
  <div id="app">
    <ev/>
    <fi/>
    <ol>
      <todoitem v-bind:key="item.id" v-bind:todo="item" v-for="item in groceryList"/>
    </ol>
  </div>
</template>

<script>
import ev from './components/events.vue'
import fi from './components/fine.vue'
import todoitem from './components/todo-item.vue'
export default {
  name: 'app',
  components: {
    ev,
    fi,
    todoitem
  },
  data () {
  return {
      groceryList: [
        { id: 0, text: '蔬菜' },
        { id: 1, text: '奶酪' },
        { id: 2, text: '随便其它什么人吃的东西' }
      ]
    }

}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
