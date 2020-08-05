<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item">
        <img class="item-img" src="http://img1.qunarzz.com/sight/p0/1501/f4/f467729126949c3a.water.jpg_140x140_ef235b1c.jpg" alt="">
        <div class="item-info">
          <p class="item-title">标题标题标题标题标题</p>
          <p class="item-desc">利益点</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend'
}
</script>

<style lang="stylus" scoped>
.title
  line-height .8rem
  text-indent .2rem
  background #eee
.item
  display flex
  height 1.9rem
  background red
  .item-img
    width 1.7rem
    height 1.7rem
    padding .1rem
</style>
