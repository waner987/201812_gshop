<template>
  <div class="search">
    <HeaderTop title="搜索"></HeaderTop>
    <form action="#" class="search_form">
      <input type="search" name="search" placeholder="请输入商家或美食名称" class="search_input">
      <input type="submit" name="submit" class="search_submit">
    </form>

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
  .search
    width 100%
    height 100%
    overflow hidden

    .search_form
      clearFix()
      margin-top 44px
      background-color #fff
      padding 12px 8px
      display flex
      justify-content space-between
      .search_input
        width: 80%
        border 4px solid #f2f2f2
        font-size 14px
        color #333
        background-color #f2f2f2
      .search_submit
        width:18%
        border 4px solid #02a774
        font-size 16px
        color #fff
        background-color #02a774
</style>
