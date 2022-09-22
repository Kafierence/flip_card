<script> 
    export default{
        data(){
            return{
                
            }
        },
        props:{
            totalOfBlocks:{
                type:Number,
                require:true,
            }
        }
    }
</script>
<template>
    <div class="box_container">
        <div class="box_content">
            <div class="box_title">
                4 x 4
            </div>
        </div>
    </div>
</template>

<style scoped>
    .box_container{
       border: 6px solid beige;
    }
    .box_content{
         display: flex;
        justify-content: center;
        align-content: center;
    }
    .box_title{

    }
</style>