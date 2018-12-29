<template>
  <div class="footer_guide">
    <a class="guide_item" href="javascript:;" :class="{on:'/msite'===$route.path}" @click="goTo('/msite')">
        <span class="item_icon">
          <i class="iconfont icon-waimai"></i>
        </span>
      <span>外卖</span>
    </a>
    <a class="guide_item" href="javascript:;" :class="{on:'/search'===$route.path}" @click="goTo('/search')">
        <span class="item_icon">
          <i class="iconfont icon-search"></i>
        </span>
      <span>搜索</span>
    </a>
    <a class="guide_item" href="javascript:;" :class="{on:'/order'===$route.path}" @click="goTo('/order')">
        <span class="item_icon">
          <i class="iconfont icon-dingdan"></i>
        </span>
      <span>订单</span>
    </a>
    <a class="guide_item" href="javascript:;" :class="{on:'/profile'===$route.path}" @click="goTo('/profile')">
        <span class="item_icon">
          <i class="iconfont icon-geren"></i>
        </span>
      <span>我的</span>
    </a>

  </div>
</template>

<script>
  export default {
    name: "FooterGuide",
    methods: {
      goTo(path){
        this.$router.replace(path)
      }
    }
  }
</script>

<style scoped lang='stylus' rel='stylesheet/stylus'>

  .footer_guide
    top-border-1px(#e4e4e4)
    position fixed
    bottom 0
    left 0
    z-index: 100
    width: 100%
    height 48px
    display flex
    background-color #fff

    .guide_item
      display flex
      flex-direction: column
      text-align center
      align-items center
      margin: 5px
      flex 1
      &.on
        color #02a774
      span
        font-size 12px
        margin-top 2px
        margin-bottom 2px
        .iconfont
          font-size 18px
</style>
