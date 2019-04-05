<template>
  <div class="hello">
    <!-- 导航栏 -->
    <div class="naver">
      <div class="logo" ><img src="./img/多边形 1.png"></div>
      <div class="naver-box">
      <div class="naver-block" ><span class="naver-block-font">首页</span> <div class="naver-block-rectangle"></div> </div>
       <div class="naver-block" ><span class="naver-block-font">精品肉类</span><div class="naver-block-rectangle"></div> </div>
        <div class="naver-block" ><span class="naver-block-font">禽类蛋品</span><div class="naver-block-rectangle"></div> </div>
         <div class="naver-block" ><span class="naver-block-font">海鲜水产</span> <div class="naver-block-rectangle"></div></div>
          <div class="naver-block" ><span class="naver-block-font">关于我们</span> <div class="naver-block-rectangle"></div></div>
    </div>
    <div class="sign-in"> <span class='sign'>[注册]</span> <span class='in'>[登录]</span></div>
    </div>
    <div class="logo2" ></div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.logo{
  width: 50px;
  height:50px;

  position: relative;
  float: left;
  left: 20%;
}
.logo2{
 width: 50px;
  height:50px;
  background-color: red;
  position: absolute;
 top:0px;
 right: 20%;
}
.sign-in{
  position: absolute;
  right:24.5%;
  top:4px;
  width: 100px;
  height: 20px;
  font-size: 12px;
  color: #1e2c5d;
}
img{

height: 50px;

}
.sign{

}
.in{
  margin-left:5px; 
}
.naver{
 
position: absolute;
top:0px;
  width: 1520px;
  height: 50px;
  background-color: #fff;
}
.naver-box{
  float: left;
  left: 10.04%;
  margin-left:10%;
  position:relative;
  width: 35%;
  height: 100%;
  background-color: #fff;
}
.naver-block{
  
  color: #1c1c1e;
  font-size: 15px;
  float: left;
  text-align: center;
  position: relative;
  
  width: 20%;
  height: 100%;
  top: 0px;
  background-color: #fff;
  line-height: 60px;
}
.naver-block-rectangle{
  width: 100%;
  height: 5%;
  position: absolute;
bottom:0px;
background-color: #1e2c5d;
display: none;
left: 0px;
}
.naver-block:hover{
  background-color: #e7e8ec;
  font-size: 16px;
}

.naver-block:hover .naver-block-rectangle{
  display: inline;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
