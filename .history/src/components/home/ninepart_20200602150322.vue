<template>
 <div>
    <div class="box">
        <div class="nav">
            <div class="top">
                <div class="t-right">
                    <a href="" class="t-font">基本功</a>
                    <a href="" class="atr">行业专家打造的免费基础课程，注册即可学习</a>
                </div>
                <div>
                    <a href="" class="ta">更多>></a>
                </div>
            </div>
            <div class="foot">
                <div class="ft1">
                    <div><img src="src="https://dn-simplecloud.shiyanlou.com/courses/uid770606-20191112-1573539538032?imageView2/2/h/250"" alt=""></div>
                    <div class="ftbox"> 
                        <div>
                            <div class="ft-font">Go + Nuxt.js 搭建一个 BBS 系统</div>
                            <div></div>
                            <div></div>
                        </div>
                    </div>
                </div>
                <div class="ft1"></div>
                <div class="ft1"></div>
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
    .ft1 {
        display: flex;
    }
    .ftbox {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>