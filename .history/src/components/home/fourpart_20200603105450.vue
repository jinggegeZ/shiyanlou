<template>
  <div>
    <div class="three">
      <div class="three_a">
        <div class="three_b">
          <a href>
            <span class="three_c">楼+ 实战课程</span>精选会员项目课程，动手中收获
          </a>
          <a href>更多></a>
        </div>
        <div class="four" >
          <!-- 大块 -->
          <a href="">
            <img src="https://doc.shiyanlou.com/courses/1508/214893/a1a8820ea275202fd11473539f57c3e2-0?imageView2/2/h/250" alt="">
          </a>
          <!-- 小块 -->
          <a class="four_a" href="" v-for="(item,index) in course.courses" :key="index">
            <div class="four_b">
              <img :src="item.picture_url" alt="">
            </div>
            <div class="four_white"></div>
            <div class="four_e">
              <div>{{item.students_count}}</div>
              <div class="four_h">训练营</div>
            </div>
            <div class="four_c">
               <div class="four_f">{{item.name}}</div>
               <div class="four_d">{{item.description}}</div>
            </div>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from'axios'
export default {
  data() {
    return {
      course:[]
    };
  },
  components: {},
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