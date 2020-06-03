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
                <div class="ft1" v-for="(item,index) in arr" :key="index">
                    <a href=""><img :src="item.picture_url" alt=""></a>
                    <div class="ftbox"> 
                        <div class="ftb">
                            <a href="">{{item.name}}</a>
                            <div class="ft-font"><a href="">{{item.description}}</a></div>
                            <div class="f-foot">
                                <a href="">{{item.tags}}</a>
                                <a class="foot-font" href="">查看详情</a>
                            </div>
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
         arr:[],
     }
   },
   components: {

   },
   methods: {
       getData(){
       axios.get('http://120.78.14.107/api/v2/index/louplus').then(res => {
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
        margin-right: 25px;
    }
    .ft1 {
        display: flex;
    }
    .ftbox {
        width: 60%;
        display: flex;
        justify-content: center;
        align-items: center;
        background: white;
    }
    .ftb {
        width: 80%;
        height: 80%;
        
    }
    .ft-font {
        font-size: 14px;
        margin-top: 20px;
    }
    .f-foot {
        display: flex;
        justify-content: space-between;
        margin-top: 70px;
    }
    .foot-font {
        width: 120px;
        background: rgb(255,151,23);
        display: flex;
        justify-content: center;
        align-items: center;
        color:white;
        
    }
</style>