<template>
 <div>
      <div class="box">
          <div class="nav">
              <div class="top">
                    <div class="t-left">
                        <div class="t-font">楼+实验课程</div>
                        <div><a class="t-font2" href="">定期开班，导师助教全程辅导，最快最优成长</a></div>
                    </div>
                    <div class="t-right">
                        <a href="">更多>></a>
                    </div>
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
    a{
        text-decoration: none;
        color: white;
    }
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

</style>