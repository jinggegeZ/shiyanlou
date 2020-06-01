<template>
 <div>
  <div class="box">
    <div class="nav">
        <div class="n-right">
          <div><img src="https://static.shiyanlou.com/frontend/dist/img/9f43b00.svg" alt="">做实验，学编程</div>
        </div>
        <div class="n-left">
          <div>企业版</div>
          <div class="nl-1"></div>
          <div>学校版</div>
          <div>登陆</div>
          <div class="nl-2">注册</div>
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
   height: 60px;
   
 }
 .nav {
   width: 1200px;
   display: flex;
   justify-content: space-between;
 }
 .n-left {
   display: flex;

 }
 .nl-1 {
   width: 2px;
   height: 20px;
   background: rgb(153,153,153);
 }
</style>