<template>
  <div class="page" @click="to">
    这是列表页
  </div>
</template>

<script>
  export default{
    data(){
      return{

      }
    },
    beforeRouteEnter(to,from,next) {
      if(from.name!='detail'){
        to.meta.keepAlive=false
      }
      next()
    },
    beforeRouteLeave(to,from,next){
      if(to.name==='detail'){
        from.meta.keepAlive=true
      }
      next()
    },
    methods:{
      to:function(){
        this.$router.push({name:'detail'})
      }
    }
  }
</script>

<style scoped="scoped">
  .page{
    background: khaki;
    height: 200vh;
  }

</style>
