<script>
import imgF from "../assets/images/icon_back.png";
import imgB from "../assets/images/1.png";
export default {
    data(){
        return {isFlip:false, }
    },
    methods:{
        onHandleRote(){
            this.isFlip=!this.isFlip;
            console.log("rendering")
        }
    }
};
</script>

<template>
  <div class="card_container">
    <div class="card_content">
      <div class="card_font" v-if="isFlip==false" @click="onHandleRote">
        <img src="../assets/images/icon_back.png" alt="" />
      </div>
      <div class="card_back" v-if="isFlip==true" @click="onHandleRote">
        <img src="../assets/images/1.png" alt="" />
      </div>
    </div>
  </div>
</template>
<style lang="css" scoped>
@-webkit-keyframes spinner {
  from {
    -webkit-transform: rotateY(0deg);
  }
  to {
    -webkit-transform: rotateY(-180deg);
  }
}

.card_container {
    display: inline-block;
    margin-bottom: 1rem;
    margin-right: 1rem;
}
.card_content {
    width: 100%;
    height: 100%;
    transition: transform 1s;
    transform-style: preserve-3d;
    cursor: pointer;
    position: relative;
}
.card_font {
  position: absolute;
  padding: 1rem;
  backface-visibility: hidden;
  border: 1px solid beige;
  border-radius: 6px;
    max-width: 49.5px;

}
.card_font img {
  object-fit: contain;
  width: 100%;
  height: 100%;
}
.card_back {
    display: flex;
    align-items: center;
    justify-items: center;
    border-radius: 6px;
    max-width: 120px;
    padding: 1rem;
    position: relative;
     transform: rotateY(-180);
 
}
.card_back img{
    object-fit: contain;
  width: 100%;
  height: 100%;
}
.card_content .is_flip {
}
</style>
