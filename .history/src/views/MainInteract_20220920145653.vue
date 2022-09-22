<script> 
    export default{
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
    <h4>Number of Block {{totalOfBlock}}</h4>
</template>