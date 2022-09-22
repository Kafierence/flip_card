<script> 
import BoxVue from '../components/Box.vue';


export default{
    data(){
        return {
           totalOfBlock:0,
           
        }
    },  
    components:{
        BoxVue
    },
    methods:{
     
        /*  getSelectMode(value){
           this.totalOfBlocks=value;
           console.log(this.totalOfBlock)
          
        } */
        onSetModeValue(event,num){
            console.log(num)
            this.totalOfBlock=num;
        },
        onModeSelected(){
            this.$emit('onModeSelected',this.totalOfBlock);
        }
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
            <box-vue :totalOfBlocks="16" @numBlock="getSelectMode" @click="onSetModeValue($event,16)"/>
            <box-vue  :totalOfBlocks="32" @numBlock="getSelectMode"
            @click="onSetModeValue($event,32)"/>
            <box-vue  :totalOfBlocks="64" @numBlock="getSelectMode"
            @click="onSetModeValue($event,64)"/>
            <box-vue  :totalOfBlocks="128" @numBlock="getSelectMode"
            @click="onSetModeValue($event,128)"/>
           <!--  <box-vue  :totalOfBlocks="256" @numBlock="getSelectMode"/> -->
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
        text-transform: uppercase;
    }
    .container .title_select{
        font-size: 2rem;
        text-transform: capitalize;
    }
    .container .mode_select{
        margin-top: 5rem;
        display: flex;
        gap: 15px;
    }
</style>