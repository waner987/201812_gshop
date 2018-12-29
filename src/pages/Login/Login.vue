<template>
  <div class="login_container">
    <div class="login_inner">
      <div class="login_header">
        <h2 class="login_logo">硅谷外卖</h2>
        <div class="login_header_title">
          <a href="javascript:;" class="on">短信登陆</a>
          <a href="javascript:;" >密码登陆</a>
        </div>
      </div>
      <div class="login_content">
        <form>
          <div >
            <section class="login_message">
              <input type="text" maxlength="11" placeholder="手机号">
              <button class="get_verification" disabled="disabled">获取验证码</button>
            </section>
            <section class="login_verification">
              <input type="text" maxlength="8" placeholder="验证码">
            </section>
            <section class="login_hint">
              温馨提示：未注册硅谷外卖帐号的手机号，登录时将自动注册，且代表已同意
              <a href="javascript:;">《用户服务协议》</a>
            </section>
          </div>
          <div class="on">
            <section class="login_message">
              <input type="text" maxlength="11" placeholder="手机/邮箱/用户名">
            </section>
            <section class="login_verification">
              <input type="text" maxlength="8" placeholder="密码" >
              <input type="password" maxlength="8" placeholder="密码">
              <div class="switch_button ">
                <div class="switch_circle"></div>
                <span class="switch_text">abc</span>
              </div>
            </section>
            <section class="login_message">
              <input type="text" maxlength="11" placeholder="验证码">
              <img src="./images/captcha.svg" alt="captcha" class="get_verification">
            </section>
            <!--<section class="login_hint">-->
              <!--温馨提示：未注册硅谷外卖帐号的手机号，登录时将自动注册，且代表已同意-->
              <!--<a href="javascript:;">《用户服务协议》</a>-->
            <!--</section>-->
          </div>
          <button class="login_submit">登录</button>
        </form>
        <a href="javascript:;" class="about_us">关于我们</a>
      </div>
      <a href="javascript:" class="go_back" @click="$router.back()">
        <i class="iconfont icon-jiantou2"></i>
      </a>
    </div>
  </div>
</template>

<script>
    export default {
        name: "Login"
    }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixins.stylus"
  .login_container
    width 100%
    height 100%
    background #fff
    .login_inner
      width: 80%
      padding-top 60px
      margin:0 auto
      .login_header
        .login_logo
          font-size 40px
          font-weight bold
          color #02a774
          text-align center
        .login_header_title
          padding-top 40px
          text-align center
          >a
            color #333
            font-size 14px
            padding-bottom 4px
            display inline-block
            &:first-child
              margin-right 40px
            &.on
              color #02a774
              font-weight 700
              border-bottom 2px solid #02a774

      .login_content
        >form
          >div
            display none
            &.on
              display block
            input
              width: 100%
              height: 100%
              padding-left 10px
              outline none
              border:1px solid #ddd
              border-radius 4px
              -webkit-box-sizing: border-box
              -moz-box-sizing: border-box
              box-sizing: border-box
              font:400 14px Arial
              &:focus
                border:1px solid #02a774
            .login_message
              height 48px
              margin-top 16px
              font-size 14px
              background #fff
              position relative
              .get_verification
                position absolute
                top: 50%
                -webkit-transform: translateY(-50%)
                -moz-transform: translateY(-50%)
                -ms-transform: translateY(-50%)
                -o-transform: translateY(-50%)
                transform: translateY(-50%)
                right:10px
                outline none
                border:none
                background transparent
                color #ccc
                font-size 14px
            .login_verification
              position relative
              input
                margin-top 16px
                height 48px
                font-size 14px
                background #fff
              .switch_button
                font-size 12px
                border 1px solid #ddd
                border-radius 8px
                transition background-color .3s,border-color .3s
                padding 0 6px
                width 30px
                height 16px
                line-height 16px
                color #fff
                position absolute
                bottom: 24px
                right 10px
                transform translateY(50%)
                &.off
                  background #fff
                  .switch_text
                    float right
                    color #ddd
                &.on
                  background #02a774
                .switch_circle
                  width:16px
                  height:16px
                  border-radius 50%
                  background #fff
                  box-shadow 0 2px 4px 0 rgba(0,0,0,.1)
                  border 1px solid #ddd
                  position absolute
                  top -1px
                  left -1px
                  transition transform .3s
                  &.right
                    transform translateX(30px)
            .login_hint
              margin-top 12px
              color #999
              font-size 14px
              line-height 20px
              >a
                color #02a774

          .login_submit
            width: 100%
            height:42px
            margin-top 40px
            border-bottom 4px
            background #4cd96f
            color #fff
            text-align center
            line-height 42px
            font-size 16px
            border:0

        .about_us
          font-size 12px
          margin-top 20px
          color: #999
          display: block
          text-align center
      .go_back
        position absolute
        top 5px
        left 5px
        width 30px
        height 30px
        >.iconfont
          font-size 20px
          color #999
</style>
