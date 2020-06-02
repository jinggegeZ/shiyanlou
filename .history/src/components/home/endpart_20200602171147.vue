<template>
 <div>
    <div class="box">
        <div class="nav">  
            <div class="body">
                <div class="b-body">
                    <div><img src="https://static.shiyanlou.com/frontend/dist/img/4a4ab3d.svg" alt=""></div>
                    <div class="b-font">动手做实验，轻松学IT</div>
                    <div class="b-web">
                        <div><a href=""><img src="https://static.shiyanlou.com/frontend/dist/img/9f56dbd.png" alt="" height="50px" width="50px"></a></div>
                        <div><a href=""><img src="https://static.shiyanlou.com/frontend/dist/img/9f56dbd.png" alt="" height="50px" width="50px"></a></div>
                    </div>
                </div>
                <div class="b-body">
                    <div><a class="b-font2" href="">合作</a></div>
                    <div><a href="">关于我们</a></div>
                    <div><a href="">联系我们</a></div>
                    <div><a href="">加入我们</a></div>
                </div>
                <div class="b-body">
                    <div><a class="b-font2" href="">合作</a></div>
                    <div><a href="">关于我们</a></div>
                    <div><a href="">联系我们</a></div>
                    <div><a href="">加入我们</a></div>
                </div>
                <div class="b-body">
                    <div><a class="b-font2" href="">合作</a></div>
                    <div><a href="">关于我们</a></div>
                    <div><a href="">联系我们</a></div>
                    <div><a href="">加入我们</a></div>
                </div>
                <div class="b-body">
                    <div><a class="b-font2" href="">合作</a></div>
                    <div><a href="">关于我们</a></div>
                    <div><a href="">联系我们</a></div>
                    <div><a href="">加入我们</a></div>
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
    a {
        text-decoration: none;
        color: rgb(127,89,51);
    }
    .b-body:hover .a{
        color: white;
    }
    .box {
        width: 100%;
        display: flex;
        justify-content: center;
        background: rgb(51,51,51);
    }
    .nav{
        width: 1200px;
    }
    .body {
        display: flex;
        justify-content: space-between;
        
    }
    .b-body {
         width: 20%;
         text-align: center;
    }
    
    .b-font2 {
        color: rgb(127,89,51);
        font-size: 16px;
    }
    .b-font {
        
        font-weight: 700;
        font-style: 30px;
        color: greenyellow;
        margin-top: 10px;

    }
    .b-web {
        width: 150px;
        display: flex;
        margin-top: 10px;
        margin-left: 50px;
        justify-content: space-between;
    }
</style>