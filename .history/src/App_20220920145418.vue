<script>
  import WelcomeVue from './views/Welcome.vue';
  import MainInteractVue from './views/MainInteract.vue';
  export default{
    components:{
      WelcomeVue,
      MainInteractVue
    }
    ,methods:{
        onSelectMode(value){
          this.totalOfBlock=value;
          console.log(value);
        }
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
    <main-interact-vue />
  </template>
</template>