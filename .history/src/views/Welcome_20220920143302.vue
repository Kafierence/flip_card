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
            <box-vue :totalOfBlocks="16"/>
            <box-vue  :totalOfBlocks="32"/>
            <box-vue  :totalOfBlocks="64" />
            <box-vue  :totalOfBlocks="128"/>
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
        text-transform: capitalize;
    }
    .container .title_select{
        font-size: 2rem;
    }
    .container .mode_select{
        margin-top: 5rem;
        display: flex;
        gap: 15px;
    }
</style>