<template>
  <!--订单-->
    <div>
      <section class="order">
        <section class="order_no_login">
          <img src="./images/person.png">
          <h3>登录后查看外卖订单</h3>
          <button>立即登录</button>
        </section>
      </section>
    </div>
</template>

<script>
export default {

}

</script>
<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixins.styl"
  .order  //订单
    width 100%
    .order_no_login
      padding-top 100px
      width 60%
      margin 0 auto
      text-align center
      >img
        display block
        width 90%
        height 30%
        margin-left 13px
      >h3
        padding 10px 0
        font-size 17px
        color #6a6a6a
      >button
        display inline-block
        background #02b6fd
        font-size 14px
        color #fff
        border 0
        outline none
        border-radius 1px
        padding 10px 32px
</style>