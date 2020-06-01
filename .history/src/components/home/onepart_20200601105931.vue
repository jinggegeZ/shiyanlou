<template>
 <div>
  <div class="box">
    <div class="nav">
        <div class="n-top">
        <div class="n-right">
          <div><img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="" width="122px" height="50px"><span class="item">做实验，学编程</span></div>
        </div>
        <div class="n-left">
          <div>企业版</div>
          <div class="nl-1"></div>
          <div>学校版</div>
          <div style="color:rgb(8,191,145)">登陆</div>
          <div class="nl-2">注册</div>
        </div>
        </div>
    </div>
  </div>
 </div>
</template>

<script>
 export default {
   data () {
     return {
       
     }
   },
   components: {

   },
   methods: {

   },
   mounted() {

   },
   watch: {

   },
   computed: {

   }
 }
</script>

<style scoped>
  *{
    display: flex;
    justify-content: center;
  }
 .box {
   width: 100%;
   height: 150px;
   
 }
 .nav {
   width: 1200px;
   
 }
 .n-top {
   width: 1180px;
   height: 65px;
   display: flex;
   justify-content: space-between;
   padding: 10px;
 }
  .n-right {
    width: 250px;
    display: flex;
    align-items: center;
  }
 .n-left {
   display: flex;
    justify-content: space-around;
    width: 285px;
    align-items: center;
 }
 .nl-1 {
   width: 2px;
   height: 20px;
   background: rgb(153,153,153);
 }
 
 .item {
   height: 50px;
   display: flex;
   align-items: center;
 }
</style>