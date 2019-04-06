<template> 
    <div class='first'>


       <div class="second">
        <swiper :options="swiperOption" ref="mySwiper">
    <!-- slides -->
    <swiper-slide><img  class="img" src="./img/背景.png"></swiper-slide>
   
    <swiper-slide><img class="img" src="./img/背景1.png"></swiper-slide>
    <swiper-slide><img class="img" src="./img/背景2.png"></swiper-slide>
    <swiper-slide><img class="img" src="./img/背景3.png"></swiper-slide>
    <swiper-slide><img class="img" src="./img/背景4.png"></swiper-slide>
    
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
    <div class="swiper-button-prevv" slot="button-prev"> <img  src="./img/left.png"></div>
    <div class="swiper-button-nextt" slot="button-next">  <img  src="./img/right.png"> </div>
  </swiper>
 </div></div>
</template>
<script>
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
    
    name: 'SlideShow',
     props: {
    msg: String, },

components:{
swiper,
swiperSlide
},

    data() {
      return {
        swiperOption: {
          // some swiper options/callbacks 用了一个vue插件vue-awesom-swiper，请在main.js中写入一些数据
          // 所有的参数同 swiper 官方 api 参数
          
          pagination: {
            el: '.swiper-pagination'
          },
          navigation: {
            nextEl: '.swiper-button-nextt',
            prevEl: '.swiper-button-prevv'
          }
        }
      }
    },
    computed: {
      swiper() {
        return this.$refs.mySwiper.swiper
      }
    }
  }

</script>
<style scoped>
/* .spanB{
  position: absolute;
  text-align: center;
  bottom: 0PX;
  left: 650px;
}
span{
  width: 50px;
  height: 3px;
  position: relative;
  background-color: #fff;
  display: inline-block;
  z-index: 6;
  bottom: 0px;
  margin-left: 15px;
}
ul{
  position: relative;
  top: 0px;
  width: 1520px;
  height: 204px;
  margin-top: 0px;
  margin-left: 0px;
 
}
img{
 
  width: 912px;
  height: 300px;
}
li{
  position: absolute;
 top: 0px;
}
.list1{
transform:translateX(80px) scale(0.81);
transform-origin: 0% 100%;
}
.list2{transform: translateX(265px);
z-index: 5;
}
.list3{transform: translateX(474px) scale(0.81);
transform-origin: 100% 100%;} */
.first{
    position: absolute;
    top:50px;
    width: 1520px;
    height: 300px;
    background-color: #51648c;
    margin-top: 0px;
    padding-top: 0px;
}
.second{
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0px;
}
.img{
 top:0px;
  width: 912px;
  height: 300px;
}

.swiper-button-prevv{
      position: absolute;
    /* left: 50px; */
    top: 90px;
    width: 49px;
    height: 110px;
    left: 20%;
    margin-top: 0px;
    z-index: 10;
    cursor: pointer;
     opacity:0.5;
    background-size: 27px 44px;
    background-position: center;
    background-repeat: no-repeat;
}

.swiper-button-nextt {
    position: absolute;
    /* left: 50px; */
     top: 90px;
    width: 49px;
    height: 110px;
    right: 20%;
  opacity:0.5;
    margin-top: 0px;
    z-index: 10;
    cursor: pointer;
    
    background-size: 27px 44px;
    background-position: center;
    background-repeat: no-repeat;
    
}
</style>
