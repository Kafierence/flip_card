<script>
  import WelcomeVue from './views/Welcome.vue';
  import MainInteractVue from './views/MainInteract.vue';
  export default{
    components:{
      WelcomeVue,
      MainInteractVue
    }
    ,methods:{

    }
    ,data(){
      return {
        totalOfBlock:0,
        status:'Defaul'
      }
    }
  }
</script>
<template>  
  <template v-if="status==='Default'">
      <welcome-vue />
  </template>
  <template v-else>
    <main-interact-vue />
  </template>
</template>