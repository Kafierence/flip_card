<script>
  import WelcomeVue from './views/Welcome.vue';
  import MainInteractVue from './views/MainInteract.vue';
  export default{
    components:{
      WelcomeVue,
      MainInteractVue
    }
    ,methods:{
        onGetModeValue(value){
          this.totalOfBlock=value;
          this.status='Ready'
          console.log(value);
          console.log(this.status)
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
  <welcome-vue />
</template>