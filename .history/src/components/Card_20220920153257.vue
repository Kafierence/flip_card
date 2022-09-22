<script> 
    import imgF from '../assets/images/icon_back.png'
    import imgB from '../assets/images/1.png';
    export default{

    }
</script>

<template>
    <div class="card_container">
        <div class="card_content">
            <div class="card_font">
                <img src='../assets/images/icon_back.png' alt="">
            </div>
            <div class="card_back">
                <img src="../assets/images/1.png" alt="">
            </div>
        </div>
    </div>
</template>
<style scoped>
    .card_container{
        border: 1px solid beige;
        border-radius: 6px;
    }
    .card_content{

    }
    .card_font{
        position: absolute;
    }
    .card_font img{
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    .card_back{

    }
    .card_content .is_flip{

    }
</style>