<template>
  <div class="profile">
    <HeaderTop title="我的"></HeaderTop>
    <section class="profile_number">
      <router-link to="/login" class="profile_link">
        <div class="profile_img">
          <i class="iconfont icon-person"></i>
        </div>
        <div class="user_info">
          <div class="user_info_content">
            <p class="user_info_top">登录/注册</p>
            <p class="user_info_bottom">
              <span class="user-icon">
                   <i class="iconfont icon-shouji icon-mobile"></i>
              </span>
              <span class="icon_mobile_number">暂无绑定手机号</span>
            </p>
          </div>
          <div class="arrow">
            <i class="iconfont icon-jiantou1"></i>
          </div>
        </div>
      </router-link>
    </section>
    <section class="profile_info_data">
      <ul class="info_data_list">
        <a class="info_data_link">
          <span class="data_top">
            <span class="data_num">0.00</span>元
          </span>
          <span class="data_bottom">我的余额</span>
        </a>
        <a class="info_data_link">
          <span class="data_top">
            <span class="data_num num2">0</span>个
          </span>
          <span class="data_bottom">我的优惠</span>
        </a>
        <a class="info_data_link">
          <span class="data_top">
            <span class="data_num num3">0</span>分
          </span>
          <span class="data_bottom">我的积分</span>
        </a>
      </ul>
    </section>
    <section class="profile_function">
      <ul class="profile_function_ul">
        <a href='javascript:' class="profile_function_li">
          <span class="function_icon_left">
            <i class="iconfont icon-order-s"></i>
          </span>
          <div class="function_li_right">
            <span class="profile_function_title">我的订单</span>
            <i class="iconfont icon-jiantou1"></i>
          </div>
        </a>
        <a href='javascript:' class="profile_function_li">
          <span class="function_icon_left">
            <i class="iconfont icon-jifen"></i>
          </span>
          <div class="function_li_right">
            <span class="profile_function_title">积分商城</span>
            <i class="iconfont icon-jiantou1"></i>
          </div>
        </a>
        <a href='javascript:' class="profile_function_li">
          <span class="function_icon_left">
            <i class="iconfont icon-vip"></i>
          </span>
          <div class="function_li_right">
            <span class="profile_function_title">外卖会员卡</span>
            <i class="iconfont icon-jiantou1"></i>
          </div>
        </a>
        <a href='javascript:' class="profile_function_li">
          <span class="function_icon_left">
            <i class="iconfont icon-fuwu"></i>
          </span>
          <div class="function_li_right">
            <span class="profile_function_title">服务中心</span>
            <i class="iconfont icon-jiantou1"></i>
          </div>
        </a>
      </ul>
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
  .profile
    width 100%
    height 100%
    overflow hidden

    .profile_number
      clearFix()
      margin-top 44px
      width 100%
      overflow: hidden
      .profile_link
        background #02a774
        padding 20px 8px
        display flex
        justify-content space-between
        .profile_img
          width 60px
          height 60px
          border-radius 50%
          overflow hidden
          .icon-person
            background #e4e4e4
            font-size 62px
        .user_info
          display flex
          width 74%
          justify-content space-between
          align-items center
          color: #fff
          .user_info_content
            .user_info_top
              font-size 18px
              font-weight: 700
              margin-bottom 8px
            .user_info_bottom
              font-size 14px
              .user-icon
                display inline-block
                width 20px
                height 20px
                margin-left -15px
                margin-right 8px
                position relative
                top -4px
                .icon-mobile
                  font-size 30px
                  vertical-align text-top
              .icon_mobile_number
                font-size 14px
                color #fff

          .arrow
            .icon-jiantou1
              color #fff
              font-size 5px

    .profile_info_data
      background #fff
      width 100%
      bottom-border-1px(#e4e4e4)
      .info_data_list
        padding: 18px 8px
        display flex
        .info_data_link
          width: 33.3%
          display flex
          flex-direction column
          text-align center
          .data_top
            margin-bottom 8px
            color #333
            font-size 13px
            .data_num
              color #f90
              font-size 26px
              margin-right 4px
            .num2
              color #ff5f3e
            .num3
              color #6ac20b
          .data_bottom
            font-size 12px
            color #666

    .profile_function
      width 100%
      background #fff
      .profile_function_ul
        padding:0 8px
        .profile_function_li
          bottom-border-1px(#f1f1f1)
          padding: 10px 0
          display flex
          justify-content space-between
          align-items center
          .function_icon_left
            width 10%
            .icon-order-s
              color #02a774
              font-size 26px
            .icon-jifen
              color #ff5f3e
              font-size 30px
              margin-left -2px
            .icon-vip
              color #f90
              font-size 22px
              margin-left 2px
            .icon-fuwu
              color #02a774
              font-size 26px
          .function_li_right
            width 90%
            display flex
            justify-content space-between
            align-items center
            .profile_function_title
              font-size 14px
              color #333
            .icon-jiantou1
              color #dddddd
              font-size 8px

</style>
