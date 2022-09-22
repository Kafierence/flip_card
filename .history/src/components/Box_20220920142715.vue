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
        },
        methods:{
            onSelectMode(){
                console.log(this.totalOfBlocks)
            }
        }
    }
</script>
<template>
    <div class="box_container" @click="onSelectMode">
        <div class="box_content">
            <div class="box_title">
                16 x 16
            </div>
        </div>
    </div>
</template>

<style scoped>
    .box_container{
       border: 1px solid beige;
       border-radius: 12px;
        transition: all .3s;
    }
    .box_container:hover{
        cursor: pointer;
        background-color: beige;
        color: black;
    }
    .box_content{
         display: flex;
        justify-content: center;
        align-content: center;
    }
    .box_title{
        padding: 2.5rem 2rem;
        font-size: 24px;
    }
</style>