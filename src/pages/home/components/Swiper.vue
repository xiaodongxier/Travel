<template>
  <div class="wrapper">
    <swiper :options="swiperOptions">
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl" alt="">
      </swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default{
  name: 'HomeSwiper',
  // data: function(){
  data () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination',
        loop: true
        // pagination: {
        //   el: '.swiper-pagination'
        // }
      },
      swiperList: [{
        id: '001',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/20200501.jpg'
      },
      {
        id: '002',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/20200502.jpg'
      },
      {
        id: '003',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/20200503.jpg'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background #fff
.wrapper
  width 100%
  height 0
  overflow hidden
  padding-bottom 56.26%
  // padding-bottom 31.25%
  background #eee
  .swiper-img
    width 100%
</style>
