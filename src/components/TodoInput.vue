<template lang="ko">
    <div class="add">
        <input class="add__input" type="text" placeholder="Enter your task" v-model="newTodoItem" @keyup.enter="addTodoItem"></input>
        <button class="add__button" @click.prevent="onClickAdd">Add</button>
    </div>
</template>
<script>
export default {
    data(){
        return {
            newTodoItem: ''
        }
    },
    methods: {
        addTodoItem(){
            localStorage.setItem(this.newTodoItem, this.newTodoItem);
        },
        onClickAdd(){
            this.addTodoItem();
        }
    },
  created() {
      //
  },
  mounted() {
      //
  }

}
</script>
<style lang="ko">
    
</style>