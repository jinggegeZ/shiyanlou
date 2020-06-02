<template>
 <div>
    <div class="box">
      <div class="nav">
        <div class="body">
          <div class="item">
            <div><img src="https://static.shiyanlou.com/frontend/dist/img/5940276.gif" alt=""></div>
            <div>丰富全面的计算机实验课程</div>
          </div>
          <div class="item">
            <div><img src="https://static.shiyanlou.com/frontend/dist/img/8b66710.gif" alt=""></div>
            <div>在线编程环境，1秒启动</div>
          </div>
          <div class="item">
            <div><img src="https://static.shiyanlou.com/frontend/dist/img/9600bd2.gif" alt=""></div>
            <div>每天一个项目课，丰富你的项目经验</div>
          </div>
          <div class="item">
            <div><img src="https://static.shiyanlou.com/frontend/dist/img/7f21af6.gif" alt=""></div>
            <div>有效学习时间，真实记录你的代码生涯</div>
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

<style scoped >
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        
        background: rgb(249,249,249);
    }
    .nav{
        width: 1200px;
    }
    .body {
        display: flex;
        justify-content: space-around;
        align-items: center;
        margin-top: 50px;
        background: rgb(249,249,249);
    }
    .item {
        text-align: center;
        width: 210px;
    }
</style>