<script>
  import WelcomeVue from './views/Welcome.vue';
  export default{
    components:{
      WelcomeVue,
    }
    ,methods:{

    }
    ,data(){
      return {
        totalOfBlock:0,
        status:'Default'
      }
    }
  }
</script>
<template>  
  <welcome-vue />
</template>