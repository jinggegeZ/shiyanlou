<template>
  <div>
    <div class="box">
      <div class="nav">
        <div class="top">
          <div class="t-right">
            <a href class="t-font">近期好课</a>
            <a href class="atr">及时学习，跟进时代的脚步</a>
          </div>
          <div>
            <a href class="ta">更多>></a>
          </div>
        </div>
        <div class="f-foot">
                <swiper ref="mySwiper" :options="swiperOptions">
                <swiper-slide v-for="(item,index) in course.courses" :key="index">
                <a class="fa" href>
                <div class="ding"><img :src="item.picture_url" alt /></div>
                <div class="fa_a">
                  <div class="fa_b">{{item.name}}</div>
                  <div class="fa_c">{{item.description}}</div>
                </div>
                <div class="fa_e"></div>
                <div class="fa_d">
                        <div class="fa-f">
                        <div>
                        <img src="../pic/5.png" alt />
                        </div>
                    <div>{{item.students_count}}</div>
                  </div>
                </div>
              </a>
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
          </swiper>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/css/swiper.css";
import axios from "axios";
export default {
  data() {
    return {
      course: [],
      swiperOptions: {
        pagination: {
          el: ".swiper-pagination"
        },
        // autoplay: true,
        slidesPerView: 4,
        slidesPerGroup: 4,
      }
    };
  },
  components: {
      Swiper,
        SwiperSlide,
  },
  methods: {
    getData() {
      axios
        .get("http://120.78.14.107/api/v2/index/classfication-courses")
        .then(res => {
          this.course = res.data[1];
          console.log(res.data);
        })
        .catch(err => {
          console.log(err);
        });
    }
  },
  mounted() {
    this.getData();
  },
  watch: {},
  computed: {}
};
</script>

<style scoped>
body {
  background-color: #f9f9f9;
  color: #3a3a3a;
}
a {
  text-decoration: none;
}
.three {
  display: flex;
  justify-content: center;
}
.three_a {
  width: 1140px;
  margin-top: 30px;
}
.three_b {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 30px;
}
.three_c {
  font-size: 18px;
  color: #565656 !important;
  border-right: 1px solid #565656;
  padding-right: 10px;
  margin-right: 10px;
}
.three_b a {
  color: #666;
}
.four{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}
.four_b{
  height: 150px;
}
.four_b img{
  width: 100%;
    height: 150px;
}
.four_a{
  display: block;
  width: 262px;
  color: #666;
  position: relative;
  box-shadow: 0 2px 2px 0 #ddd;
  margin-bottom: 20px;
}
.four_a:hover{
  box-shadow: 0 4px 20px 4px #ddd;
}
.four_c{
  position: absolute;
  bottom: 53px;
  left: 0;
  width: 100%;
  height: 53px;
   transition: all 0.7s;
   background-color: white;
   overflow: hidden;
}
.four_a:hover .four_c{
  height: 123px;
}
.four_d{
    display: -webkit-box;
    overflow: hidden;
    white-space: normal !important;
    text-overflow: ellipsis;
    word-wrap: break-word;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;
   padding-left: 5px;
   background-color: white;
       transition: all 0.7s;
       font-size: 14px;
       padding: 5px;

}
.four_e{
  height: 54px;
  color: #9b9da2;
}
.four_f{
  height: 53px;
  
  line-height: 50px;
  padding-left: 5px;
}
.four_e{
  height: 53px;
  line-height: 53px;
  padding-left: 5px;
  padding-right: 5px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.four_white{
  height: 46px;
}
.four_h{
    font-size: 12px;
    background: #f66;
    color: white;
    height: 25px;
    line-height: 25px;
    border-radius: 50px;
    width: 50px;
    text-align: center;
}
</style>