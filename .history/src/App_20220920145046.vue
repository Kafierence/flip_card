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
  <template v-if="status==='Default'">
      <welcome-vue />
  </template>
  <template v-else>
    
  </template>
</template>