<script> 
import BoxVue from '../components/Box.vue';


export default{
    components:{
        BoxVue
    }
}
</script>
<template>
    <div class="container">
        <div class="title_start">
            Pokemon Memories Game
        </div>
        <div class="title_select">
            Select mode to start game
        </div>
        <div class="mode_select">
            <box-vue />
        </div>
    </div>
</template>
<style scoped>
    .container{
       color: white;
       text-align: center;

    }
    .container .title_start{
        font-size: 4rem;
    }
    .container .title_select{
        font-size: 2rem;
    }
    .container .mode_select{
        display: flex;
        
    }
</style>