<template>
  <section class="loginContainer">
      <div class="loginInner">
        <div class="login_header">
          <!-- <h2 class="login_logo">饿了么</h2> -->
          <img src="./images/TB1kHnqpcKfxu4jSZPfXXb3dXXa-750-192.png" alt="" class="login_logo">
          <div class="login_header_title">
            <a href="javascript:;" class="on">短信登录</a>
            <a href="javascript:;">密码登录</a>
          </div>
        </div>
        <div class="login_content">
          <form>
            <div class="on">
              <section class="login_message">
                <input type="tel" maxlength="11" placeholder="手机号">
                <button disabled="disabled" class="get_verification">获取验证码</button>
              </section>
              <section class="login_verification">
                <input type="tel" maxlength="8" placeholder="验证码">
              </section>
              <section class="login_hint">
                温馨提示：未注册硅谷外卖帐号的手机号，登录时将自动注册，且代表已同意
                <a href="javascript:;">《用户服务协议》</a>
              </section>
            </div>
            <div>
              <section>
                <section class="login_message">
                  <input type="tel" maxlength="11" placeholder="手机/邮箱/用户名">
                </section>
                <section class="login_verification">
                  <input type="tel" maxlength="8" placeholder="密码">
                  <div class="switch_button off">
                    <div class="switch_circle"></div>
                    <span class="switch_text">...</span>
                  </div>
                </section>
                <section class="login_message">
                  <input type="text" maxlength="11" placeholder="验证码">
                  <img class="get_verification" src="./images/captcha.svg" alt="captcha">
                </section>
              </section>
            </div>
            <button class="login_submit">登录</button>
          </form>
          <a href="javascript:;" class="about_us">关于我们</a>
        </div>
        <a href="javascript:" class="go_back" @click="$router.go(-1)">
          <i class="el-icon-arrow-left"></i>
        </a>
      </div>
    </section>
</template>

<script>
export default {
  
}

</script>
<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixins.styl"
  .loginContainer
    width 100%
    height 100%
    background #fff
    .loginInner
      padding-top 60px
      width 80%
      margin 0 auto
      .login_header
        text-align center
        .login_logo
          text-align center
          width 142px
          height 36px
        .login_header_title
          padding-top 40px
          text-align center
          >a
            color #333
            font-size 14px
            padding-bottom 4px
            &:first-child
              margin-right 40px
            &.on
              color #02b6fd
              font-weight 700
              border-bottom 2px solid #02b6fd
      .login_content
        >form
          >div
            display none
            &.on
              display block
            input
              width 100%
              height 100%
              padding-left 10px
              box-sizing border-box
              border 1px solid #ddd
              border-radius 4px
              outline 0
              font 400 14px Arial
              &:focus
                border 1px solid #02b6fd
            .login_message
              position relative
              margin-top 16px
              height 48px
              font-size 14px
              background #fff
              .get_verification
                position absolute
                top 50%
                right 10px
                transform translateY(-50%)
                border 0
                color #ccc
                font-size 14px
                background transparent
            .login_verification
              position relative
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
                top 50%
                right 10px
                transform translateY(-50%)
                &.off
                  background #fff
                  .switch_text
                    float right
                    color #ddd
                &.on
                  background #02a774
                >.switch_circle
                  //transform translateX(27px)
                  position absolute
                  top -1px
                  left -1px
                  width 16px
                  height 16px
                  border 1px solid #ddd
                  border-radius 50%
                  background #fff
                  box-shadow 0 2px 4px 0 rgba(0,0,0,.1)
                  transition transform .3s
            .login_hint
              margin-top 12px
              color #999
              font-size 14px
              line-height 20px
              >a
                color #02b6fd
          .login_submit
            display block
            width 100%
            height 42px
            margin-top 30px
            border-radius 4px
            background #02b6fd
            color #fff
            text-align center
            font-size 16px
            line-height 42px
            border 0
            border-radius 21px
        .about_us
          display block
          font-size 12px
          margin-top 20px
          text-align center
          color #999
      .go_back
        position absolute
        top 10px
        left 5px
        width 30px
        height 30px
        >.el-icon-arrow-left
          font-size 25px
          color #999
</style>