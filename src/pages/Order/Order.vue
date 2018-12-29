<template>
  <div class="order">
    <HeaderTop title="订单"></HeaderTop>
    <section class="order_no_login">
      <img src="./images/person.png">
      <h3>登录后查看外卖订单</h3>
      <button>立即登陆</button>
    </section>
  </div>
</template>

<script>
  import HeaderTop from '../../components/HeaderTop/HeaderTop'

  export default {
    name: "FooterGuide",
    components:{
      HeaderTop
    }
  }
</script>

<style scoped lang='stylus' rel='stylesheet/stylus'>
  @import "../../common/stylus/mixins.stylus"
  .order
    width 100%
    height 100%
    overflow hidden

    .order_no_login
      padding-top 140px
      text-align center
      width 60%
      margin 0 auto
      > img
        width 100%
        height 30%
      > h3
        padding 10px 0
        font-size 17px
        color #6a6a6a
      > button
        display inline-block
        outline: 0
        border: 0
        background #02a774
        font-size 14px
        color #fff
        padding 6px 12px
        border-radius 4px
</style>
