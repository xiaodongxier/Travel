<template>
  <div class="header">
    <!--
      高度 86px
      左边宽度 60px
      右边宽度 128px
      -->
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe6aa;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
      display flex
      line-height 0.86rem
      background $bgColor
      color #fff
      .header-left
        width: 0.64rem
        float: left
        .back-icon
          text-align center
          font-size .4rem
      .header-input
        flex: 1
        height .64rem
        line-height .64rem
        padding-left .2rem
        margin-top .11rem
        margin-left .2rem
        border-radius .1rem
        background #fff
        color #ccc
      .header-right
        width 1.24rem
        float right
        text-align center
        .arrow-icon
          font-size .24rem
          margin-left -.05rem
</style>
