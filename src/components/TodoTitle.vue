<template lang="ko">
    <div class="title">
        <p class="title__message">{{message}}</p>
        <p class="title__task">
            You've got
            <span class="title__task-total">{{taskTotal}}</span> task today.
        </p>
        <h1>사랑하는 사람, 우리 가족들, 행복하길...</h1>
    </div>
    </div>
</template>
<script>
export default {
    data(){
        return {
            taskTotal:0
        }
    },
  methods:{

  }
}
</script>
<style lang="ko">
    
</style>