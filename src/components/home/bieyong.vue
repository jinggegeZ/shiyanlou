<template>
 <div>

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
<div class="f-foot">
                        <a class="fa" href="">
                        <div class="">
                            <img src="https://dn-simplecloud.shiyanlou.com/courses/uid214893-20200426-1587870364389?imageView2/2/h/150/q/100" alt="">
                        </div>
                        <div class="fa_a">
                            <div class="fa_b">TypeScript 基础入门</div>
                            <div class="fa_c">
                            本课程是 TypeScript 基础入门课程。课程从什么是Ty
                            peScript 开始，一步步讲解到基本数据类型、接口、类
                            、函数、模块、命名空间等知识点。
                            </div>
                        </div>
                        <div class="fa_e"></div>
                        <div class="fa_d">
                            <div class="fa-f">
                                <div><img src="../pic/5.png" alt=""></div>
                                <div>135</div>
                            </div>
                            <div class="fa-g">训练营</div>
                        </div>
                        </a>
                        <a class="fa" href="">
                        <div class="">
                            <img src="https://dn-simplecloud.shiyanlou.com/courses/uid214893-20200426-1587870364389?imageView2/2/h/150/q/100" alt="">
                        </div>
                        <div class="fa_a">
                            <div class="fa_b">TypeScript 基础入门</div>
                            <div class="fa_c">
                            本课程是 TypeScript 基础入门课程。课程从什么是Ty
                            peScript 开始，一步步讲解到基本数据类型、接口、类
                            、函数、模块、命名空间等知识点。
                            </div>
                        </div>
                        <div class="fa_e"></div>
                        <div class="fa_d">
                            <div class="fa-f">
                                <div><img src="../pic/5.png" alt=""></div>
                                <div>135</div>
                            </div>
                            <div class="fa-g">训练营</div>
                        </div>
                        </a>
                        <a class="fa" href="">
                        <div class="">
                            <img src="https://dn-simplecloud.shiyanlou.com/courses/uid214893-20200426-1587870364389?imageView2/2/h/150/q/100" alt="">
                        </div>
                        <div class="fa_a">
                            <div class="fa_b">TypeScript 基础入门</div>
                            <div class="fa_c">
                            本课程是 TypeScript 基础入门课程。课程从什么是Ty
                            peScript 开始，一步步讲解到基本数据类型、接口、类
                            、函数、模块、命名空间等知识点。
                            </div>
                        </div>
                        <div class="fa_e"></div>
                        <div class="fa_d">
                            <div class="fa-f">
                                <div><img src="../pic/5.png" alt=""></div>
                                <div>135</div>
                            </div>
                            <div class="fa-g">训练营</div>
                        </div>
                        </a>
                        <a class="fa" href="">
                        <div class="">
                            <img src="https://dn-simplecloud.shiyanlou.com/courses/uid214893-20200426-1587870364389?imageView2/2/h/150/q/100" alt="">
                        </div>
                        <div class="fa_a">
                            <div class="fa_b">TypeScript 基础入门</div>
                            <div class="fa_c">
                            本课程是 TypeScript 基础入门课程。课程从什么是Ty
                            peScript 开始，一步步讲解到基本数据类型、接口、类
                            、函数、模块、命名空间等知识点。
                            </div>
                        </div>
                        <div class="fa_e"></div>
                        <div class="fa_d">
                            <div class="fa-f">
                                <div><img src="../pic/5.png" alt=""></div>
                                <div>135</div>
                            </div>
                            
                        </div>
                        </a>

                    </div>
                    <a class="fa" href="" v-for="(item,index) in arr.courses" :key="index">
                                <div v-if="index < 2">
                                        <div class=""><img :src="item.picture_url" alt=""></div>
                                    <div class="fa_a">
                                    <div class="fa_b">{{item.name}}</div>
                                    <div class="fa_c">{{item.description}}</div>
                                    </div>
                                    <div class="fa_e"></div>
                                    <div class="fa-f">
                                    <div><img src="../pic/5.png" alt=""></div>
                                    <div>{{item.students_count}}</div>
                                     </div>
                                </div>

                        </a>
</style>