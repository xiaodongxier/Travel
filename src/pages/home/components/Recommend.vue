<!--
 * @Author: wangyongjie
 * @Date: 2020-08-05 21:34:37
 * @LastEditors: wangyongjie
 * @LastEditTime: 2020-08-08 21:53:55
 * @e-mail: admin@xiaodongxier.com
 * @FilePath: /Travel/src/pages/home/components/Recommend.vue
-->
<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="(item,index) of titleList" :key="index">
        <img class="item-img" :src="item.imgUrl" alt="">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data: function () {
    return {
      titleList: [{
        id: '001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1501/f4/f467729126949c3a.water.jpg_140x140_ef235b1c.jpg',
        title: '1标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题',
        desc: '1利益点'
      },
      {
        id: '002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1501/f4/f467729126949c3a.water.jpg_140x140_ef235b1c.jpg',
        title: '2标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题',
        desc: '2利益点'
      },
      {
        id: '003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1501/f4/f467729126949c3a.water.jpg_140x140_ef235b1c.jpg',
        title: '3标题标题标题标题标题标题标题标题标题标题标题标题标题标题标题',
        desc: '3利益点'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
@import '~styles/mixins.styl'
.title
  line-height .8rem
  text-indent .2rem
  background #eee
.item
  display flex
  height 1.9rem
  // background red
  .item-img
    width 1.7rem
    height 1.7rem
    padding .1rem
  .item-info
    flex 1
    padding .1rem
    min-width 0
    .item-title
      line-height .54rem
      font-size .32rem
      ellipsis()
    .item-desc
      line-height .4rem
      ellipsis()
    .item-button
      color #fff
      line-height .44rem
      margin-top .16rem
      background #ff9300
      padding 0 .2rem
      border-radius .06rem
</style>
