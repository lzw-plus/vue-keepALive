<template>
  <div class="page" @click="to">
    
  </div>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods:{
    to:function(){
      this.$router.push({name:'list'})
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .page{
    background: salmon;
    height: 100vh;
  }
</style>
