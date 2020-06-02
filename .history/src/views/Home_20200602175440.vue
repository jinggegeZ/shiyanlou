<template>
 <div>
    <onepart></onepart>
    <twopart></twopart>
    <threepart></threepart>
    <fourpart></fourpart>
    <fivepart></fivepart>
    <sixpart></sixpart>
    <sevenpart></sevenpart>
    <eightpart></eightpart>
    <ninepart></ninepart>
    <tenpart></tenpart>
    <elevenpart></elevenpart>
    <endpart></endpart>
 </div>
</template>

<script>
import onepart from '../components/home/onepart'
import twopart from '../components/home/twopart'
import threepart from '../components/home/threepart'
import fourpart from '../components/home/fourpart'
import fivepart from '../components/home/fivepart'
import sixpart from '../components/home/sixpart'
import sevenpart from '../components/home/sevenpart'
import eightpart from '../components/home/eightpart'
import ninepart from '../components/home/ninepart'
import tenpart from '../components/home/tenpart'
import elevenpart from '../components/home/elevenpart'
import endpart from '../components/home/endpart'
import { Swiper, SwiperSlide,} from 'vue-awesome-swiper'
import 'swiper/css/swiper.css'
import axios from 'axios'
 export default {
   data () {
     return {
       pics:[]
     }
   },
   components: {
     onepart,
     twopart,
     threepart,
     fourpart,
     fivepart,
     sixpart,
     sevenpart,
     eightpart,
     ninepart,
     tenpart,
     elevenpart,
     endpart,
     Swiper,
    SwiperSlide,
   },
   methods: {
     getData(){
       axios.get('http://120.78.14.107/api/v2/index/banner-pictures').then(res => {
         console.log(res.data);
       }).catch(err => {
         console.log(err);
       })
     }
   },
   mounted() {
     this.getData()
   },
   watch: {

   },
   computed: {
     
   }
 }
</script>

<style scoped lang='scss'>

</style>
