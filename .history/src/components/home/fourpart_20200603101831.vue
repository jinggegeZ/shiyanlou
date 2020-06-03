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
                        <a href="" class="ta">更多>></a>
                    </div>
                </div>
                <div class="foot">
                    <div class="f-top">
                        <a href="" class="ft1">
                        <img src="https://doc.shiyanlou.com/courses/1508/214893/a1a8820ea275202fd11473539f57c3e2-0?imageView2/2/h/250" alt="">
                        </a>
                        <!--  -->
                        <a class="fa" href="" v-for="(item,index) in courses" :key="index">
                                <div class=""><img :src="item.courses.picture_url" alt=""></div>
                                <div class="fa_a">
                                <div class="fa_b">{{item.courses.name}}</div>
                                <div class="fa_c">{{item.courses.description}}</div>
                                </div>
                                <div class="fa_e"></div>
                                <div class="fa-f">
                                <div><img src="../pic/5.png" alt=""></div>
                                <div>{{item.courses.students_count}}</div>
                                </div>
                        </a>
                        </div>
                    </div>
                    
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
       axios.get('http://120.78.14.107/api/v2/index/classfication-courses').then(res => {
         this.arr = res.data[0]
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

<style scoped>
    a{
        text-decoration: none;
        color: black;
    }
    .ta {
        margin-right: 10px;
    }
  .box {
        width: 100%;
        display: flex;
        justify-content: center;
        
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
        margin-bottom: 10px;
    }
    .f-foot {
        display: flex;
        justify-content: space-around;
        position: relative;
    }
    .fa{
        position: relative;
        margin-bottom: 10px;
        
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

</style>