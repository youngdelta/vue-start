<template lang="ko">
    <div class="title">
        <p class="title__message">{{message}}</p>
        <p class="title__task">
            You've got
            <span class="title__task-total">{{taskTotal}}</span> task today.
        </p>
    </div>
</template>
<script>
export default {
    data(){
        return {
            taskTotal:0
        }
    }
}
</script>
<style lang="ko">
    
</style>