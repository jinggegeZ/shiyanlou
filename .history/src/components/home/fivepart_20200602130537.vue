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

<style scoped >
    a {
        text-decoration: none;
        color: black;
    }
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        margin-top: 10px;
        background: rgb(249,249,249);
    }
    .nav{
        width: 1180px;
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
        margin-right: 10px;
    }
</style>