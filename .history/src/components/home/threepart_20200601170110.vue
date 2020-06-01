<template>
 <div>
        <div class="box">
            <div class="nav">
                <div class="top">
                    <div class="t-left">
                        <div class="t-font">楼+实验课程</div>
                        <a class="t-font2" href="">定期开班，导师助教全程辅导，最快最优成长</a>
                    </div>
                    <div class="t-right">
                        <a href="">更多>></a>
                    </div>
                </div>
                <div class="foot">
                    <a class="f-box" href="">
                        <div><img src="https://dn-simplecloud.shiyanlou.com/course/1552548603751_1545727521555_imglouplusML.png" alt="" height="90px"></div>
                        <div>6周成为机器学习初级工程师</div>
                        <div>最近班次：6月2日</div>
                    </a>
                    <a class="f-box" href="">
                        <div></div>
                        <div></div>
                        <div></div>
                    </a>
                    <a class="f-box" href=""></a>
                    <a class="f-box" href=""></a>
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
        display: flex;
        justify-content: center;
        margin-top: 10px;
    }
    .nav{
        width: 1180px;
    }
    .top {
        display: flex;
        justify-content: space-between;
    }
    .t-left {
        height: 80px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .t-font {
        font-weight: 700;
        font-size: 24px;
    }
    .t-font2 {
        border-left:2px solid black;
        margin-left: 10px;
        padding-left: 10px;
    }
    a{
        text-decoration: none;
        color: black;
    }
    .t-right {
        height: 80px;
        display: flex;
        align-items: center;
    }
    .foot {
        display: flex;
        justify-content: space-around;
    }
    .f-box {
        width: 22%;
        display: flex;
        
        align-items: center;
        height: 200px;
        border-radius: 10px;
        box-shadow: 0 1px 2px 0 #ddd;
        overflow: hidden;
        flex-wrap: wrap;
    }
    .f-box:hover{
        box-shadow: 0 1px 30px 0 #d2d2d2;
    }
</style>