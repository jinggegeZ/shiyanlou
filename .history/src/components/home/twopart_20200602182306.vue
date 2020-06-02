<template>
 <div>
    <div class="box">
        <div class="mildle">
            <div class="left">
                <div class="l-item">
                    <div class="item">
                        <a class="item-a" href="">后端开发</a>
                        <a class="item-a" href="">Python</a>
                        <a class="item-a" href="">PHP</a>
                    </div>
                    <div class="item-b">
                            <div class="itemb-1">后端开发</div>
                            <div class="itemb-2">
                                <a class="itemb-3">Python</a>
                                <a class="itemb-3">Python</a>
                            </div>
                            <div class="itemb-1">课程推荐</div>
                        </div>
                </div>
                <div class="l-item">
                    <div class="item">
                        <a class="item-a" href="">Linux运维</a>
                        <a class="item-a" href="">Linux</a>
                        <a class="item-a" href="">Shell</a>
                    </div>
                    <div class="item-b">
                            <div class="itemb-1">Linux运维</div>
                            <div class="itemb-2">
                                <a class="itemb-3">Python</a>
                                <a class="itemb-3">Python</a>
                            </div>
                            <div class="itemb-1">课程推荐</div>
                        </div>
                </div>
                <div class="l-item">
                    <div class="item">
                        <a class="item-a" href="">云计算与大数据</a>
                        <a class="item-a" href="">Hadoop</a>
                        <a class="item-a" href="">Spark</a>
                    </div>
                    <div class="item-b">
                            <div class="itemb-1">云计算与大数据</div>
                            <div class="itemb-2">
                                <a class="itemb-3">Python</a>
                                <a class="itemb-3">Python</a>
                            </div>
                            <div class="itemb-1">课程推荐</div>
                        </div>
                </div>
            </div>
        </div>
        <div class="b-foot">
            <swiper ref="mySwiper" :options="swiperOptions">
                <swiper-slide v-for="(item,index) in pics" :key="index">
                <div class="beibei" :style="{background:item.background_color}">
                <img :src="item.picture_url" alt="">
                </div>
                </swiper-slide>
                <div class="swiper-pagination" slot="pagination"></div>
            </swiper>
        </div>
    </div>
 </div>
</template>

<script>
import { Swiper, SwiperSlide,} from 'vue-awesome-swiper'
import 'swiper/css/swiper.css'
import axios from 'axios'
 export default {
   data () {
     return {
         pics:[],
         swiperOptions: {
          pagination: {
            el: '.swiper-pagination'
          },
          
        }
     }
   },
   components: {
        Swiper,
        SwiperSlide,
   },
   methods: {
       getData(){
       axios.get('http://120.78.14.107/api/v2/index/banner-pictures').then(res => {
         this.pics = res.data
         console.log(res.data);
       }).catch(err => {
         console.log(err);
       })
     }
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
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        
        
        height: 515px;
    }
    .mildle {
        width: 1200px;
        z-index: 99;
        height: 100%;
        
    }
    .b-foot {
        width: 100%;

    }
    .left {
        width: 260px;
        background: rgba(0,0,0,.18);
        
    }
    .l-item {
        display:flex;
        justify-content: center;
        position: relative;
    }
    .l-item:hover{
         background: white;
    }
    .l-item:hover .item-b{
         visibility: visible;
    }
    .item:hover .item-a{
        color: #666;
       
    }
    .item {
        display: flex;
        width: 240px;
        height: 50px;
        align-items: center;
        justify-content: space-around;
        border-bottom: 1px solid white;
    }
    .item-a {
        color: white;
    }
    .item-a:hover{
        color:#08bf91 !important;
    }
    a{
        text-decoration: none;
    }
    .item-b {
        width: 300px;
        height: 300px;
        position: absolute;
        background: white;
        top: 0;
        left: 260px;
        visibility: hidden;
    }
    .itemb-1 {
        margin-left: 20px;
        width: 100px;
        height: 30px;
        background: rgb(238,238,238);
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 10px;
        font-size: 14px;
    }
    .itemb-2 {
        margin-left: 20px;
        margin-top: 10px;
        display: flex;
    }
    
    .itemb-3 {
        color: black;
        border-left: 1px solid black;
        padding: 2px;
    }
    .itemb-3:hover{
      color:#08bf91;
    }
</style>