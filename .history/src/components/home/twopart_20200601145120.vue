<template>
 <div>
    <div class="box">
        <div class="mildle">
            <div class="left">
                <div class="l-item">
                    <div class="item">
                        <a class="item-a" href="">后端开发</a>
                        <a class="item-a" href="">Python</a>
                        <a class="item-a" href="">PHP</a>
                    </div>
                </div>
                <div class="l-item">
                    <div class="item">
                        <a class="item-a" href="">Linux运维</a>
                        <a class="item-a" href="">Linux</a>
                        <a class="item-a" href="">Shell</a>
                    </div>
                </div>
                <div class="l-item">
                    <div class="item">
                        <a class="item-a" href="">云计算与大数据</a>
                        <a class="item-a" href="">Hadoop</a>
                        <a class="item-a" href="">Spark</a>
                    </div>
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
        padding-left: 10px;
    }
    .left {
        width: 260px;
        background: rgba(0,0,0,.18);
    }
    .l-item {
        display:flex;
        justify-content: center;
    }
    .l-item:hover{
         background: white;
    }
    .item:hover .item-a{
        color: black;
    }
    .item-a:hover{
        color: #08bf91;
    }
    .item {
        display: flex;
        width: 240px;
        height: 50px;
        align-items: center;
        justify-content: space-around;
        position: relative;
        border-bottom: 1px solid white;
    }
    .item-a {
        color: white;
    }
    a{
        text-decoration: none;
    }
</style>