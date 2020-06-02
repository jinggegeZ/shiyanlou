<template>
 <div>
    <div class="box">  
        <div class="nav">
            <div class="top">
                <div class="t-right">
                    <a href="" class="t-font">后端开发</a>
                    
                </div>
                <div>
                    <a href="" class="ta">更多>></a>
                </div>
            </div>
            <div class="f-foot">
                <div>
                    <a href="">
                        <img src="https://dn-simplecloud.shiyanlou.com//assets/1590648950895_1597竖版宣传图.png?imageView2/2/h/520" alt="">
                    </a>
                </div>
                <div>
                    <div class="ff">
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
                            <div class="fa_e"></div>
                            <div class="fa_d">
                                <div class="fa-f">
                                    <div><img src="../pic/5.png" alt=""></div>
                                    <div>135</div>
                                </div>
                            </div>
                        </a>
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
                            <div class="fa_e"></div>
                            <div class="fa_d">
                                <div class="fa-f">
                                    <div><img src="../pic/5.png" alt=""></div>
                                    <div>135</div>
                                </div>
                            </div>
                        </a>
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
                            <div class="fa_e"></div>
                            <div class="fa_d">
                                <div class="fa-f">
                                    <div><img src="../pic/5.png" alt=""></div>
                                    <div>135</div>
                                </div>
                            </div>
                        </a>
                    </div>
                    <div></div>
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
    a {
        text-decoration: none;
        color: black;
    }
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        
        background: rgb(249,249,249);
    }
    .nav{
        width: 1200px;
    }
    .top {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .t-right {
        display: flex;
        align-items: center;
        height: 80px;
    }
    .t-font {
        font-size: 20px;
        font-weight: 700;
    }
    .atr {
        border-left: 2px solid black;
        margin-left: 10px;
        padding-left: 10px;
    }
    .ta {
        margin-right: 10px;
    }
    .f-foot {
        display: flex;
        justify-content: space-around;
        position: relative;
    }
    .fa{
        position: relative;
        margin-top: 10px;
    }
    .fa_a{
        position: absolute;
        left: 0;
        width: 100%;
        height: 46px;
        background-color: white;
        bottom: 53px;
        overflow: hidden;
        transition: all 0.7s;
    }
    .fa_b{
        height: 46px;
        line-height: 46px;
        padding-left: 5px;
    }
    .fa_c {
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 3;
        -webkit-box-orient: vertical;
    }
    .fa_d{
        height: 53px;
        display: flex;
        align-items: center;
        padding-left: 5px;
        justify-content: space-between;
    }
    .fa_e{
        height: 46px;
    }
    .fa-f {
        display: flex;
        align-items: center;
    }
    .fa-g {
        border-radius: 15px;
        background: #f66;
        color: white;
        padding: 3px 10px;
    }
    .fa:hover .fa_a{
        height: 120px;
        
    }
    .fa:hover {
        box-shadow: 0 1px 30px 0 #d2d2d2 !important;
    }
    .ff {
        display: flex;
        justify-content: space-around;
    }
</style>