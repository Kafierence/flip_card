<script>
import imgF from "../assets/images/icon_back.png";
import imgB from "../assets/images/1.png";
export default {
    data(){
        isFlip:false,


    },
    methods:{
        
    }
};
</script>

<template>
  <div class="card_container">
    <div class="card_content">
      <div class="card_font">
        <img src="../assets/images/icon_back.png" alt="" />
      </div>
      <div class="card_back">
        <img src="../assets/images/1.png" alt="" />
      </div>
    </div>
  </div>
</template>
<style scoped>
@-webkit-keyframes spinner {
  from {
    -webkit-transform: rotateY(0deg);
  }
  to {
    -webkit-transform: rotateY(-180deg);
  }
}

.card_container {
}
.card_content {
  width: 120px;
}
.card_font {
  position: absolute;
  padding: 1rem;
  backface-visibility: hidden;
  border: 1px solid beige;
  border-radius: 6px;
  max-width: 120px;
}
.card_font img {
  object-fit: contain;
  width: 100%;
  height: 100%;
}
.card_back {
  position: relative;
  transform: rotateY(-180);
  display: none;
}
.card_content .is_flip {
}
</style>
