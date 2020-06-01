<template>
 <div>
    <div class="box">
        <div class="mildle">
            <div class="left">
                <div class="item">
                    <div>后端开发</div>
                    <div>Python</div>
                    <div>PHP</div>
                </div>
                <div class="item">
                    <div>Linux运维</div>
                    <div>Linux</div>
                    <div>Shell</div>
                </div>
                <div class="item">
                    <div>云计算与大数据</div>
                    <div>Hadoop</div>
                    <div>Spark</div>
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
        margin-top: 5px;
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
    }
</style>