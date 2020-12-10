<template>
  <!--我的-->
    <div>
      <section class="profile">
        <section class="profile-number">
          <router-link to="/login" class="profile-link">
            <div class="profile_image">
              <!-- <i class="el-icon-platform-eleme"></i> -->
              <img src="./images/ing.png" alt="" class="el-icon-platform-eleme">
            </div>
            <div class="user-info">
              <p class="user-info-top">登录/注册</p>
              <p>
                <span class="user-icon">
                  <i class="iconfont icon-shouji icon-mobile"></i>
                </span>
                <span class="icon-mobile-number"><i class="el-icon-mobile-phone"></i>登录后享受更多特权</span>
              </p>
            </div>
            <span class="arrow">
              <i class="el-icon-arrow-right"></i>
            </span>
          </router-link>
        </section>
        <section class="profile_info_data border-1px">
          <ul class="info_data_list">
            <a href="javascript:" class="info_data_link">
              <span class="info_data_top"> <span><i class="el-icon-collection"></i></span> </span>
              <span class="info_data_bottom">红包</span>
            </a>
            <!-- <a href="javascript:" class="info_data_link">
              <span class="info_data_top"><span>0</span>个</span>
              <span class="info_data_bottom">我的优惠</span>
            </a> -->
            <a href="javascript:" class="info_data_link">
              <span class="info_data_top"> <span><i class="el-icon-coin"></i></span> </span>
              <span class="info_data_bottom">金币</span>
            </a>
          </ul>
        </section>
        
        <section class="profile_my_order border-1px">
          <!-- 我的地址 -->
          <a href="javascript:" class="my_order">
            <span>
              <i class="el-icon-location-information"></i>
            </span>
            <div class="my_order_div">
              <span>我的地址</span>
              <span class="my_order_icon">
                <i class="el-icon-arrow-right"></i>
              </span>
            </div>
          </a>
        </section>
        
        <section class="profile_my_mrn border-1px">
          <!-- 金币商城 -->
          <a href="javascript:" class="my_order">
            <span>
              <i class="el-icon-shopping-bag-2"></i>
            </span>
            <div class="my_order_div">
              <span>金币商城</span>
              <span class="my_order_icon">
                <i class="el-icon-arrow-right"></i>
              </span>
            </div>
          </a>
        </section>
        <section class="profile_my_order border-1px">
          <!-- 我的客服 -->
          <a href='javascript:' class="my_order">
            <span>
              <i class="el-icon-service"></i>
            </span>
            <div class="my_order_div">
              <span>我的客服</span>
              <span class="my_order_icon">
                <i class="el-icon-arrow-right"></i>
              </span>
            </div>
          </a>
          <!-- 下载饿了么APP -->
          <a href='javascript:' class="my_order border-1px">
            <span>
              <i class="el-icon-platform-eleme"></i>
            </span>
            <div class="my_order_div">
              <span>下载饿了么APP</span>
              <span class="my_order_icon">
                <i class="el-icon-arrow-right"></i>
              </span>
            </div>
          </a>
          <!-- 规则中心 -->
          <a href="javascript:" class="my_order border-1px">
            <span>
              <i class="el-icon-document"></i>
            </span>
            <div class="my_order_div">
              <span>规则中心</span>
              <span class="my_order_icon">
                <i class="el-icon-arrow-right"></i>
              </span>
            </div>
          </a>
        </section>
        <div class="Privacy">隐私政策</div>
      </section>
    </div>
</template>

<script>
export default {

}

</script>
<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixins.styl"
  .profile //我的
    width 100%
    overflow hidden
    .profile-number
      // margin-top 45.5px
      .profile-link
        clearFix()
        position relative
        display block
        background-image linear-gradient(90deg,#0af,#0085ff)
        padding 20px 10px
        .profile_image
          float left
          width 60px
          height 60px
          border-radius 50%
          overflow hidden
          vertical-align top
          .el-icon-platform-eleme
            width 60px
            height 60px
        .user-info
          float left
          margin-top 8px
          margin-left 15px
          p
            font-weight: 700
            font-size 20px
            color #fff
            &.user-info-top
              padding-bottom 8px
            .user-icon
              display inline-block
              margin-left -28px
              // margin-right 5px
              width 20px
              height 20px
              .icon-mobile
                font-size 30px
                vertical-align text-top
            .icon-mobile-number
              font-size 12px
              color #fff
              // .el-icon-mobile-phone
        .arrow
          width 12px
          height 12px
          position absolute
          right 15px
          top 40%
          .el-icon-arrow-right
            color #fff
            font-size 10px
    .profile_info_data
      bottom-border-1px(#e4e4e4)
      width 100%
      background #fff
      overflow hidden
      .info_data_list
        clearFix()
        .info_data_link
          float left
          width 49.7%
          text-align center
          border-right 1px solid #f1f1f1
          .info_data_top
            display block
            width 100%
            font-size 14px
            color #333
            padding 15px 5px 10px
            >span
              margin-top 10px
              width 25px
              height 25px
              display inline-block
              border-radius 50%
              background rgb(255, 95, 62)
              text-align center
              .el-icon-collection
                font-size 16px
                color #fff
                margin-top 4px
          .info_data_bottom
            display inline-block
            font-size 12px
            color #666
            font-weight bold
            padding-bottom 10px
            margin-left 10px
            margin-bottom 10px
        .info_data_link:nth-of-type(2)
          .info_data_top
            >span
              width 25px
              height 25px
              display inline-block
              border-radius 50%
              background rgb(106, 194, 11)
              text-align center
              .el-icon-coin
                font-size 16px
                color #fff
                margin-top 4px
        .info_data_link:nth-of-type(3)
          border 0
          .info_data_top
            span
              color #6ac20b
    .profile_my_order
      top-border-1px(#e4e4e4)
      margin-top 10px
      background #fff
      .my_order
        display flex
        align-items center
        padding-left 15px
        >span
          display flex
          align-items center
          width 20px
          height 20px
          >.el-icon-location-information,.el-icon-service,.el-icon-platform-eleme,.el-icon-document
            margin-left -5px
            font-size 20px
            color rgb(74, 165, 240)
        .my_order_div
          width 100%
          border-bottom 1px solid #f1f1f1
          padding 18px 10px 18px 0
          font-size 16px
          color #333
          display flex
          justify-content space-between
          span
            display block
          .my_order_icon
            width 10px
            height 10px
            .icon-jiantou1
              color #bbb
              font-size 10px
    .profile_my_mrn
      top-border-1px(#e4e4e4)
      margin-top 10px
      background #fff
      .my_order
        display flex
        align-items center
        padding-left 15px
        >span
          display flex
          align-items center
          width 20px
          height 20px
          >.el-icon-shopping-bag-2
            margin-left -5px
            font-size 20px
            color rgb(148, 217, 74)
        .my_order_div
          width 100%
          border-bottom 1px solid #f1f1f1
          padding 18px 10px 18px 0
          font-size 16px
          color #333
          display flex
          justify-content space-between
          span
            display block
          .my_order_icon
            width 10px
            height 10px
            .icon-jiantou1
              color #bbb
              font-size 10px
    .Privacy
      text-align center 
      margin: 6.133333vw auto;
      color: #4da6f0;
      font-size: .9rem;   
</style>