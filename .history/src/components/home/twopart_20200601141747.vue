<template>
 <div>
    <div class="box">
        <div class="mildle">
            <div class="left">
                <div class="item">
                    <div class="item-a">后端开发</div>
                    <div class="item-a">Python</div>
                    <div class="item-a">PHP</div>
                </div>
                <div class="item">
                    <div class="item-a">Linux运维</div>
                    <div class="item-a">Linux</div>
                    <div class="item-a">Shell</div>
                </div>
                <div class="item">
                    <div class="item-a">云计算与大数据</div>
                    <div class="item-a">Hadoop</div>
                    <div class="item-a">Spark</div>
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
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        background: rgb(255,204,51);
        margin-top: 10px;
    }
    .mildle {
        width: 1200px;
        padding: 10px;
    }
    .left {
        width: 260px;
        
    }
    .item {
        display: flex;
        color: white;
        height: 50px;
        align-items: center;
        justify-content: space-around;
        position: relative;
    }
</style>