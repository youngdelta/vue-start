<template lang="">
    <div>
        <>
        <h1>무궁화 꽃이 피었습니다.</h1>
        <div>
            가족 행복 사람
        </div>
        <hr>
        <div>
            <div>
                <span>
                    1.무병장수
                </span>
            </div>
            <div>
                <div>
                    2.어린이
                </div>
            </div>
        </div>
        <div>
          <h2>{{name}}</h2>
        </div>
        <hr>
        <ul>
          <li>list</li>
        </ul>
        <div>
          <span>test</span>
        </div>
        <hr>
        <div>
            <div>
                <span>오징어 게임</span>
            </div>
        </div>
        <div>
          <div>
            <ul>
              <li></li>
              <li></li>
              <li></li>
              <li></li>
            </ul>
          </div>
        </div>
    </div>
</template>
<script>
export default {

    data() {
    return {
      name : '무궁화',
      list:[],
      params:[],

    }
  },
  methods:{
    setName(name) {
        this.name = name;
    }
    getList() {
      console.log('getList.....');
    }
  },
    computed: {

    },
    watch: {
        
    }
    
}
</script>
<style lang="">
    
</style>