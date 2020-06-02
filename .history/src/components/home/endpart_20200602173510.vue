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
                    <div class="b-font2">公司</div>
                    <div><a href="">关于我们</a></div>
                    <div><a href="">联系我们</a></div>
                    <div><a href="">加入我们</a></div>
                </div>
                <div class="b-body">
                    <div class="b-font2">合作</div>
                    <div><a href="">成为作者</a></div>
                    <div><a href="">教室合作</a></div>
                    <div><a href="">友情链接</a></div>
                    <div><a href="">开发者</a></div>
                </div>
                <div class="b-body">
                    <div class="b-font2">服务</div>
                    <div><a href="">企业版</a></div>
                    <div><a href="">实战训练营</a></div>
                    <div><a href="">会员服务</a></div>
                    <div><a href="">实验报告</a></div>
                    <div><a href="">常见问题</a></div>
                    <div><a href="">隐私条款</a></div>
                </div>
                <div class="b-body">
                    <div class="b-font2">学习路径</div>
                    <div><a href="">Python学习路径</a></div>
                    <div><a href="">Linux学习路径</a></div>
                    <div><a href="">大数据学习路径</a></div>
                    <div><a href="">Java学习路径</a></div>
                    <div><a href="">PHP学习路径</a></div>
                    <div><a href="">全部</a></div>
                </div>
            </div>
        </div>
    </div>
    <div class="foot">
        <div class="ft-box">
            <div class="ft-font">Copyright @2013-2020 实验楼在线教育 | 蜀ICP备13019762号</div>
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
        color: #999;
    }
    a:hover {
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
        margin-top: 20px;
    }
    .b-body {
         width: 20%;
         text-align: center;
    }
    .b-body a {
        display: block;
        margin-bottom: 5px;
    }
    .b-font2 {
        color: #999;
        font-size: 20px;
        margin-bottom: 20px;
        display: block;
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
    .foot {
        width: 100%;
        background: black;
    }
    .ft-box {
        
        display: flex;
        justify-content: center;
        align-items: center;
        height: 50px;
    }
    .ft-font {
        color: white;
    }
</style>