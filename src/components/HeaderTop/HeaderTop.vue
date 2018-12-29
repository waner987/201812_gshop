<template>
  <div class="header">
    <!--<span class="header_search">-->
      <!--<i class="iconfont icon-sousuo"></i>-->
    <!--</span>-->
    <slot name="left"></slot>
    <span class="header_title">
      <span class="header_title_text">{{title}}</span>
    </span>
    <slot name="right"></slot>
    <!--<span class="header_login">-->
      <!--<span class="header_login_text">登录|注册</span>-->
    <!--</span>-->
  </div>
</template>

<script>
  export default {
    name: "HeaderTop",
    props:{
      title:String
    }
  }
</script>

<style scoped lang='stylus' rel='stylesheet/stylus'>
  @import "../../common/stylus/mixins.stylus"

    .header
      bottom-border-1px(#02c186)
      position fixed
      width: 100%
      height 44px
      /*line-height 24px*/
      background $green
      color: white
      padding 8px 8px
      -webkit-box-sizing: border-box
      -moz-box-sizing: border-box
      box-sizing: border-box
      z-index 100
      line-height 28px
      clearFix()

      .header_title
        width: 180px
        text-align center
        overflow hidden
        white-space nowrap
        -ms-text-overflow: ellipsis
        text-overflow: ellipsis
        position absolute
        transform translate(-50%, -50%)
        top 50%
        left 50%
      .header_login
        font-size 12px
        position absolute
        transform translate(0, -50%)
        top 50%
        right:8px
</style>
