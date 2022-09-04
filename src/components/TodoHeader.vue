<template lang="ko">
    <header class="header">
        <h1 class="logo">My Todo</h1>
        <h1 class="date">{{timestamp}}</h1>
    </header>
</template>
<script>
export default {
    data(){
        return{
            timestamp:"",
        }
    },
    created() {
        const now = new Date();
        const month  = now.getMonth()+1;
        const date = now.getDate();
        const weekList = new Array('Sun.', 'Mon.','Tue.','Wed.', 'Thu.','Fri.','Sat.');
        const week = weekList[now.getDay()];
        this.timestamp = `${month}/${date} ${week}`;
    }
}
</script>
<style lang="ko">
    
</style>