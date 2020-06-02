<template>
 <div>
    <div class="box">
        <div class="box_aaa">
        <div class="mildle">
            <div class="left">
                <div class="l-item" v-for="(item,index) in arr" :key="index">
                    <div class="item">
                        <a class="item-a" href="">{{item.name}}</a>
                        <a class="item-a" href="">{{item.tags[0].name}}</a>
                        <a class="item-a" href="">{{item.tags[1].name}}</a>
                    </div>
                    <div class="item-b" >
                            <div class="itemb-1"></div>
                            <div class="itemb-2">
                                <a class="itemb-3"></a>
                                <a class="itemb-3"></a>
                            </div>
                            <div class="itemb-1"></div>
                        </div>
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
         arr:[],
         pics:[],
         swiperOptions: {
          pagination: {
            el: '.swiper-pagination'
          },
          autoplay:true,
          
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
     },
     getData1(){
       axios.get('http://120.78.14.107/api/v2/index/categories').then(res => {
         this.arr = res.data
         console.log(res.data);
       }).catch(err => {
         console.log(err);
       })
     }
   },
   mounted() {
       this.getData(),
       this.getData1()
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
        
        position: relative;
        height: 515px;
    }
    .box_aaa{
        width: 100%;
        z-index: 99;
        height: 100%;
        position: absolute;
        left: 0;
        top: 0;
        display: flex;
        justify-content: center;
    }
    .mildle {
        width: 1200px;
        
    }
    .b-foot {
        width: 100%;

    }
    .left {
        width: 260px;
        background: rgba(0,0,0,.18);
        height: 102%;
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
        height: 58px;
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
    .beibei{
        text-align: center;
        width: 100%;
        height: 100%;
    }
</style>