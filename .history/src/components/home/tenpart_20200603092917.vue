<template>
 <div>
    <div class="box">  
        <div class="nav">
            <div class="top">
                <div class="t-right">
                    <a href="" class="t-font">近期好课</a>
                    <a href="" class="atr">及时学习，跟进时代的脚步</a>
                </div>
                <div>
                    <a href="" class="ta">更多>></a>
                </div>
            </div>
            <div class="f-foot">
                    <a class="fa" href="">
                        <div class=""><a href="">
                        <img src="https://dn-simplecloud.shiyanlou.com/course/1555406408145_【路径】-【Python研发工程师】.png" alt="">
                        </a>    
                        </div>
                       <div class="ff">
                            <div class="f-font"><a href="">Python 研发工程师</a></div>
                            <div><a href="">57门课程</a></div>
                       </div>
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
       axios.get('http://120.78.14.107/api/v2/index/bootcamps').then(res => {
         this.arr = res.data
         console.log(res.data);
       }).catch(err => {
         console.log(err);
       })
   },
   },
   mounted() {
       this.getData()
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
        margin-right: 25px;
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
    .ff {
        text-align: center;
    }
    .f-font {
        font-size: 24px;
        margin-top: 15px;
        margin-bottom: 15px;
    }
    .fa:hover .fa_a{
        height: 120px;
        
    }
    .fa:hover {
        box-shadow: 0 1px 30px 0 #d2d2d2 !important;
    }
</style>