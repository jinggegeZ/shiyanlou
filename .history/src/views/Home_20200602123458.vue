<template>
 <div>
    <onepart></onepart>
    <twopart></twopart>
    <threepart></threepart>
    <fourpart></fourpart>
    <fivepart></fivepart>
 </div>
</template>

<script>
import onepart from '../components/home/onepart'
import twopart from '../components/home/twopart'
import threepart from '../components/home/threepart'
import fourpart from '../components/home/fourpart'
import fivepart from '../components/home/fivepart'
 export default {
   data () {
     return {

     }
   },
   components: {
     onepart,
     twopart,
     threepart,
     fourpart,
     fivepart,
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

<style scoped lang='scss'>

</style>
