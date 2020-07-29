<template>
  <div class="header">
    <!--
      高度 86px
      左边宽度 60px
      右边宽度 128px
      -->
    <div class="header-ledt">返回</div>
    <div class="header-input">内容</div>
    <div class="header-rig">城市</div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
    .header
        display flex
        height 0.86rem
        .header-left
          width: 0.64rem
          float: left
        .header-right
          width: 1.24rem
          float: right
        .header-input
          flex: 1
</style>
