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
                        <a class="fa" href="">
                        <div class="">
                            <img src="https://dn-simplecloud.shiyanlou.com/courses/uid214893-20200426-1587870364389?imageView2/2/h/150/q/100" alt="">
                        </div>
                        <div class="fa_a">
                            <div class="fa_b">TypeScript 基础入门</div>
                            <div class="fa_c">
                            本课程是 TypeScript 基础入门课程。课程从什么是Ty
                            peScript 开始，一步步讲解到基本数据类型、接口、类
                            、函数、模块、命名空间等知识点。
                            </div>
                        </div>
                        <div class="fa_d">123</div>
                        <div class="fa_e"></div>
                        </a>
                        
                    </div>
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
    .ftbox {
        width: 264px;
        background: white;
        position: relative;
        
    }
    .fimg {
        height: 30px;
        display: flex;
        align-items: center;
        z-index: 22;
        position: absolute;
        bottom: 0;
        left: 10px;
    }
    .ffont {
        font-size: 20px;
        margin-top: 20px;
    }
    .ftb {
        position: absolute;
        top: 10px;
    }
    .fa{
        position: relative;
    }
    .fa_a{
        position: absolute;
        left: 0;
        width: 100%;
        height: 46px;
        background-color: pink;
        bottom: 53px;
        overflow: hidden;
    }
    .fa_b{
        height: 46px;
        line-height: 46px;
        padding-left: 5px;
    }
    .fa_d{
        height: 53px;
        background-color: red;
    }
    .fa_e{
        height: 46px;
    }

</style>