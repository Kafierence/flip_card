<script> 
import CardVue from '../components/Card.vue';
    export default{
        components:{
            CardVue,
        },
        props:{
            totalOfBlock:{
                type:Number,
                require:true
            }
        }
    }
</script>

<template>
    <h2>Default Main Interact</h2>
    <h4>Number of Block {{this.totalOfBlock}}</h4>
</template>