<template>
  <div class="icons">
    <swiper>
      <swiper-slide>
        <div class="icon" v-for="item of iconList" :key="item.id">
          <div class="icon-img">
            <img class="icon-img-content" :src="item.imgUrl" alt="">
          </div>
          <p class="icon-desc">{{item.desc}}</p>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
export default{
  name: 'HomeIcons',
  data: function () {
    return {
      iconList: [{
        id: '0001',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/piao.png',
        desc: '景点门票'
      },
      {
        id: '0002',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/train.png',
        desc: '滑雪集结'
      },
      {
        id: '0003',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/hotel.png',
        desc: '泡温泉'
      },
      {
        id: '0004',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/train.png',
        desc: '动植物园'
      },
      {
        id: '0005',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/package.png',
        desc: '景点门票'
      },
      {
        id: '0006',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/flight.png',
        desc: '滑雪集结'
      },
      {
        id: '0007',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/train.png',
        desc: '泡温泉'
      },
      {
        id: '0008',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/package.png',
        desc: '动植物园'
      },
      {
        id: '0009',
        imgUrl: 'http://oss.xiaodongxier.com/gome/test/flight.png',
        desc: '动植物园'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/varibles.styl';
.icons >>> .swiper-container
  width 100%
  height 0
  padding-bottom 50%
.icon
  width 25%
  height 0
  padding-bottom 25%
  float left
  overflow hidden
  position relative
  .icon-img
    position absolute
    top 0
    left 0
    right 0
    bottom .44rem
    box-sizing border-box
    padding .1rem
    .icon-img-content
      display block
      height 100%
      margin 0 auto
  .icon-desc
    position absolute
    left 0
    right 0
    bottom 0
    height .44rem
    line-height .44rem
    text-align center
    color $darkTextColor
</style>
