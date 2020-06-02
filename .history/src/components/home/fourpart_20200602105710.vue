<template>
 <div>
      <div class="box">
          <div class="nav">
              <div class="top">
                    <div class="t-left">
                        <div class="t-font">精选项目课</div>
                        <div><a class="t-font2" href="">精选会员项目课程，动手中收获</a></div>
                    </div>
                    <div class="t-right">
                        <a href="">更多>></a>
                    </div>
                </div>
                <div class="foot">
                    <div class="f-top">
                        <a href="" class="ft1">
                        <img src="https://doc.shiyanlou.com/courses/1508/214893/a1a8820ea275202fd11473539f57c3e2-0?imageView2/2/h/250" alt="">
                        </a>
                        <!--  -->
                        <a href="">
                        <div class="">
                        <img src="" alt=""></div>
                        <div class=""></div>
                        <div class=""></div>
                        </a>
                        <!--  -->
                        
                    </>
                    <div class="f-foot"></div>
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
    a{
        text-decoration: none;
        color: black;
    }
  .box {
        width: 100%;
        display: flex;
        justify-content: center;
        margin-top: 10px;
        background: rgb(249,249,249);
    }
    .nav{
        width: 1180px;
    }
    .top {
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 80px;
    }
    .t-left {
        display: flex;
    }
    .t-font {
        font-size: 20px;
        font-weight: 700;
    }
    .t-font2 {
        border-left: 2px solid black;
        margin-left: 10px;
        padding-left: 10px;
    }
    .f-top {
        display: flex;
        justify-content: space-around;
        position: relative;
    }
    .f-foot {
        display: flex;
        justify-content: space-around;
        
    }
    
</style>