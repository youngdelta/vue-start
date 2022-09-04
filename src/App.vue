<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <hr>
    <todo-header></todo-header>
    <todo-title></todo-title>
    <TodoInput></TodoInput>
    <TodoController></TodoController>
    <TodoList></TodoList>
    <todo-footer></todo-footer>
    <hr>
    <router-view/>
  </div>
</template>

<script>
  import TodoController from "./components/TodoController.vue";
  import TodoTitle from "./components/TodoTitle.vue";
  import TodoInput from "./components/TodoInput.vue";
  import TodoHeader from "./components/TodoHeader.vue";
  import TodoFooter from "./components/TodoFooter.vue";
  import TodoList from "./components/TodoList.vue";

  export default {
    name: "app",
    components: {
    TodoHeader,
    TodoTitle,
    TodoInput,
    TodoController,
    TodoFooter,
    TodoList,
    TodoHeader,
    TodoController,
    TodoList
},
    data(){
      return {
        todo:'Hello',
      }
    },
    created(){
      this.getTodo();
    },
    mounted() {
      //

    },
    methods: {
      getTodo() {
        console.log(this.todo);
      }
    }
  }

</script>

<style>
  /* 
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
 */


</style>


