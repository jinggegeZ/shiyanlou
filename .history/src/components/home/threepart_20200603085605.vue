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
                        <a href="" class="ta">更多>></a>
                    </div>
                </div>
                <div class="foot">
                    <a class="f-box" href="">
                        <div><img src="https://dn-simplecloud.shiyanlou.com/course/1552548603751_1545727521555_imglouplusML.png" alt="" height="100px"></div>
                        <div class="f-font">6周成为机器学习初级工程师</div>
                        <div>最近班次：6月2日</div>
                    </a>
                    <a class="f-box" href="">
                        <div><img src="https://dn-simplecloud.shiyanlou.com/course/1571375889048_企业微信截图_9bd1350f-ec15-415b-b53e-e62c29ec647f.png" height="100px" alt=""></div>
                        <div class="f-font">4周掌握Python基础</div>
                        <div>最近班次：随到随学</div>
                    </a>
                    <a class="f-box" href="">
                        <div><img src="https://dn-simplecloud.shiyanlou.com/course/1565168718677_楼——首页.png" alt="" height="100px"></div>
                        <div class="f-font">6周成为深度学习工程师</div>
                        <div>最近班次：7月6日</div>
                    </a>
                    <a class="f-box" href="">
                        <div><img src="https://dn-simplecloud.shiyanlou.com/course/1552548866160_企业微信截图_15525486809695.png" alt="" height="100px"></div>
                        <div class="f-font">11周成为Python初级工程师</div>
                        <div>最近班次：5月9日</div>
                    </a>
                </div>
            </div>
        </div>
 </div>
</template>

<script>
import axios from 'axios'
 export default {
   data () {
     return {
         arr:[],
     }
   },
   components: {

   },
   methods: {
       getData(){
       axios.get('http://120.78.14.107/api/v2/index/louplus').then(res => {
         this.pics = res.data
         console.log(res.data);
       }).catch(err => {
         console.log(err);
       })
   },
   mounted() {
       this.getData(),
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
        background: rgb(249,249,249);
    }
    .nav{
        width: 1180px;
    }
    .top {
        display: flex;
        justify-content: space-between;
    }
    .ta {
        margin-right: 20px;
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
        justify-content: space-between;
    }
    .f-box {
        width: 22%;
        display: flex;
        align-items: center;
        border-radius: 10px;
        box-shadow: 0 1px 2px 0 #ddd;
        overflow: hidden;
        flex-wrap: wrap;
    }
    .f-box:hover{
        box-shadow: 0 1px 30px 0 #d2d2d2;
    }
    .f-font {
        line-height: 45px;
        font-size: 18px;
        font-weight: 700;
        text-align: center;
    }
</style>