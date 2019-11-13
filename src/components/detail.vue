<template>
  <div class="page" @click="back">
    这是详情页
  </div>
</template>

<script>
  export default{
    data(){
      return{

      }
    },
    methods:{
      back:function(){
        this.$router.go(-1)
      }
    }
  }
</script>

<style scoped="scoped">
  .page{
    background: greenyellow;
    height: 100vh;

  }
</style>
