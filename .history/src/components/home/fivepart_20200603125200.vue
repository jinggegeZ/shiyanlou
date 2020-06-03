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
            <swiper ref="mySwiper" :options="swiperOptions">
                <swiper-slide v-for="(item,index) in course.courses" :key="index">
                    <div class="fa_aa">
                    <!--  -->
                    <a class="fa" href="">
                        <div class="">
                            <img :src="item.picture_url" alt="">
                        </div>
                        <div class="fa_a">
                            <div class="fa_b">{{item.name}}</div>
                            <div class="fa_c">
                            {{item.description}}
                            </div>
                        </div>
                        <div class="fa_e"></div>
                        <div class="fa_d">
                            <div class="fa-f">
                                <div><img src="../pic/5.png" alt=""></div>
                                <div>{{item.students_count}}</div>
                            </div>
                            
                        </div>
                    </a>
                    </div>
                </swiper-slide>
                <div class="swiper-pagination" slot="pagination"></div>
            </swiper>

            
            </div>
        </div>
    </div>
 </div>
</template>

<script>
import axios from'axios'
import { Swiper, SwiperSlide,} from 'vue-awesome-swiper'
import 'swiper/css/swiper.css'
 export default {
   data () {
     return {
         course:[],
         swiperOptions: {
          pagination: {
            el: '.swiper-pagination'
          },
          autoplay:true,
          slidesPerView : 4,
            slidesPerGroup : 4,
          
        }
     }
   },
   components: {
       Swiper,
        SwiperSlide,
   },
   methods: {
        getData() {
      axios.get("http://120.78.14.107/api/v2/index/classfication-courses")
        .then(res => {
          this.course = res.data[0]
          console.log(res.data);
        })
        .catch(err => {
          console.log(err);
        });
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
    .fa_aa{
        display: flex;
        flex-wrap: wrap;
    }
</style>
