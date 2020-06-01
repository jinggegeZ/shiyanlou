<template>
 <div>
        <div class="box">
            <div class="nav">
                <div class="top">
                    <div class="t-left">
                        <div class="t-font">楼+实验课程</div>
                        <div class="t-font2">定期开班，导师助教全程辅导，最快最优成长</div>
                    </div>
                    <div></div>
                </div>
                <div class="foot"></div>
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
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        margin-top: 10px;
    }
    .nav{
        width: 1200px;
    }
    .top {
        display: flex;
        justify-content: space-between;
    }
    .t-left {
        height: 50px;
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
        margin-left: 5px;
    }
</style>