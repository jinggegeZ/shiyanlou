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