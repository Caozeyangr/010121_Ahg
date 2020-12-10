<template>
  <footer class="footer_guide">
    <a href="javascript:;" class="guide_item" :class="{on: '/home'===$route.path}" @click="goTo('/home')">
      <span class="item_icon">
        <i class="el-icon-eleme"></i>
      </span>
      <span>外卖</span>
    </a>
    <a href="javascript:;" class="guide_item" :class="{on:'/find'===$route.path}" @click="goTo('/find')">
      <span class="item_icon">
        <i class="el-icon-discover"></i>
      </span>
      <span>发现</span>
    </a>
    <a href="javascript:;" class="guide_item" :class="{on: '/order'===$route.path}" @click="goTo('/order')">
      <span class="item_icon">
        <i class="el-icon-s-order"></i>
      </span>
      <span>订单</span>
    </a>
    <a href="javascript:;" class="guide_item" :class="{on: '/profile'===$route.path}" @click="goTo('/profile')">
      <span class="item_icon">
        <i class="el-icon-user-solid"></i>
      </span>
      <span>我的</span>
    </a>
  </footer>
</template>

<script>
export default {
  methods: {
    goTo (path) {
      this.$router.replace(path)
    }
  }
};
</script>
<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixins.styl"
  .footer_guide  //footer
    top-border-1px(#e4e4e4)
    position fixed
    z-index 100
    left 0
    right 0
    bottom 0
    background-color #fff
    width 100%
    height 50px
    display flex
    .guide_item
      display flex
      flex 1
      text-align center
      flex-direction column
      align-items center
      margin 5px
      color #999999
      &.on
        color #0089dc
      span
        font-size 12px
        margin-top 2px
        margin-bottom 2px
        .el-icon-eleme,.el-icon-discover,.el-icon-s-order,.el-icon-user-solid
          font-size 22px
</style>