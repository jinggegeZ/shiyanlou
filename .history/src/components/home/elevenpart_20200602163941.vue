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
            <div></div>
          </div>
          <div class="item"></div>
          <div class="item"></div>
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
    }
</style>