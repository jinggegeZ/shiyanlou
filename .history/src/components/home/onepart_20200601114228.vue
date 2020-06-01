<template>
 <div>
  <div class="box">
    <div class="nava">
        <div class="n-top">
          <div class="n-right">
          <div><img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="" width="122px" height="50px"></div>
          <span class="item">做实验，学编程</span>
          </div>
          <div class="n-left">
            <div class="nl">企业版</div>
            <div class="nl-1"></div>
            <div class="nl">学校版</div>
            <div class="nl-3">登陆</div>
            <div class="nl-2" >注册</div>
          </div>
        </div>
        <div class="n-foot">
        <div class="nf1">
          <a class="anf" href="https:409236083@qq.com">全部课程</a>
        </div>
        <div></div>
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
  
 .box {
   width: 100%;
   height: 150px;
   background: rgb(249,249,249);
   display:flex;
   justify-content: center;
 }
 .nava{
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
    width: 300px;
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
 .nl-2 {
   height: 50px;
   width: 50px;
    background: rgb(8,191,145);
    display: flex;
    align-items: center;
    color:white;
    justify-content: center;
 }
 .item {
   height: 50px;
   display: flex;
   align-items: center;
 }
 .nl:hover{
   color:#08bf91;
 }
 .nl-3{
   color: #08bf91;
 }
 .nl-3:hover{
   color: black;
 }
 .n-foot {
   width: 1180px;
   height: 55px;
   display: flex;
   align-items: center;
   padding: 10px;
 }
 .nf1 {
   width: 260px;
   height: 55px;
   background: rgb(84,193,133);
   display: flex;
   align-items: center;
 }
 .anf{
   color:white;
   padding-left: 15px;
 }
</style>