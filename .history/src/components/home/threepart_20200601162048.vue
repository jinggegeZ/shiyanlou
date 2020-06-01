<template>
 <div>
        <div class="box">
            <div class="nav">
                <div class="top">
                    <div class="t-left">
                        <div></div>
                        <div></div>
                        <div></div>
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
        display: flex;
    }
</style>