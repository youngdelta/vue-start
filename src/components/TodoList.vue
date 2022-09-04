<template lang="ko">
    <ul class="list">
        <li class="list__item" v-for="(todoItem, index) in todoItems" :key="todoItem">
            <input type="checkbox" id="list0item-i"></input>
            <label for="list-item-1">
                <p class="list__text">Smile! :)</p>
            </label>
            <p class="list__date">5/26</p>
            <button class="list__delete" @click="removeTodo({todoItem,index})">Delete</button>
        </li>
    </ul>
</template>
<script>
export default {
    name: 'TodoList',
    data() {
        return {
            todoItems:[]
        }
    },
    created(){
        localStorage && localStorage.length > 0 && (_=>{
            // for (const key in localStorage) {
            for(let i=0;i<localStorage.length;i++) {
                if (localStorage.key(i) !== 'loglevel:webpack-dev-server') {
                    this.todoItems.push(localStorage.getItem(localStorage.key(i)));
                }
                /* 
                // console.log(key);
                if (Object.hasOwnProperty.call(localStorage, key)) {
                    const element = localStorage[key];
                    console.log(element);
                    this.todoItems.push(element)
                }
                 */
            }
        })();
    },
    methods: {
        removeTodo: "removeOneItem",
        toggleComplete: "toggleOneItem"
    },
}
</script>
<style lang="ko">
    
</style>