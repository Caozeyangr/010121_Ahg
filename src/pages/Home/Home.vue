<template>
    <!--首页外卖-->
    <section class="msite">
      <!--首页头部-->
      <header class="msite_header">
        <span class="header_search">
          <i class="el-icon-location"></i>
        </span>
        <span class="header_title">
          <span class="header_title_text ellipsis">冀中职业学院</span>
        </span>
        <span class="header_login">
         <i class="el-icon-caret-bottom"></i>
        </span>
        <span class="header_input">
          <input type="text" placeholder="搜索饿了么商家、商品名称">
        </span>
        <span class="header_inlog">
          <i class="el-icon-search"></i>
        </span>
      </header>
      <!--首页导航-->
      <nav class="msite_nav">
        <div class="swiper-container">
          <div class="swiper-wrapper">
            <div class="swiper-slide">
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/a867c870b22bc74c87c348b75528djpeg.jpg">
                </div>
                <span>美食</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/b02bd836411c016935d258b300cfejpeg.jpg">
                </div>
                <span>大牌惠吃</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/bceb19258e3264e64fb856722c3c1jpeg.jpg">
                </div>
                <span>跑腿代购</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/432619fb21a40b05cd25d11eca02djpeg.jpg">
                </div>
                <span>汉堡披萨</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/696aa5cf9820adada9b11a3d14bf5jpeg.jpg">
                </div>
                <span>甜品饮品</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/1.jpg">
                </div>
                <span>地方小吃</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/185f7259ebda19e16123884a60ef2jpeg.jpg">
                </div>
                <span>米粉面馆</span>
              </a>
              <a href="javascript:" class="link_to_food">
                <div class="food_container">
                  <img src="./images/nav/0fb469b2da210827ec16896e00420jpeg.jpg">
                </div>
                <span>炸鸡炸串</span>
              </a>
            </div>
          </div>
          <div class="swiper-pagination"></div>
        </div>
      </nav>
      <!-- 首页vip套餐 -->
      <div class="Set_meal">
        <div class="index-3xB2N_0">
          <div class="index-Q3GS5_0_index-1xT5J">
            <h3 class="index-1qvN6_0">品质套餐</h3>
            <div class="index-2W67h_0">搭配齐全吃得好</div>
            <div class="index-1DFa7_0">立即抢购> </div>
            <img src="./images/nav/df43e7e53f6e1346c3fda0609f1d3png.png" alt="" class="img">
          </div>
          <div class="index-3eoZ-_0">
            <div class="index-3M-d6_0"></div>
              <img src="./images/nav/4dd212d831becab6e3ebd484c0941jpeg.png" alt="" class="king">
              <span class="index-M9mXY_0">超级会员</span>
              <span class="index-tO6Fz_0">·&nbsp;每月领20元红包</span>
              <span class="going">立即开通></span>
          </div>
        </div>
      </div>
      <!--首页推荐商家-->
      <div class="msite_shop_list">
        <div class="shop_header">
          <i class="iconfont icon-xuanxiang"></i>
          <span class="shop_header_title">——&nbsp;&nbsp;推荐商家&nbsp;&nbsp;——</span>
        </div>
        <div class="shop_search">
          <ul class="ul_search">
            <li class="li_search">综合排序 <i class="el-icon-caret-bottom"></i></li>
            <li class="li_search">距离最近</li>
            <li class="li_search">销量最高</li>
            <li class="li_search">筛选 <i class="el-icon-table-lamp"></i></li>
          </ul>
        </div>
        <ShopList/>
      </div>
    </section>
</template>

<script>
import ShopList from '../../components/ShopList/ShopList.vue'
export default {
  components: {
    ShopList
  }
}

</script>
<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/mixins.styl"
  .msite  //首页
    width 100%
    .msite_header
      background-image linear-gradient(90deg,#0af,#0085ff)
      position fixed
      z-index 100
      left 0
      top 0
      width 100%
      height 100px
      .header_search
        position absolute
        left 12px
        top 45px
        transform translateY(-50%)
        width 10%
        height 50%
        .el-icon-location
          font-size 18px
          color #fff
      .header_title
        position absolute
        top 30px
        left 85px
        transform translate(-50%, -50%)
        width 50%
        color #fff
        text-align center
        .header_title_text
          font-size 17px
          height 20px
          color #fff
          display block
          font-weight bold
      .header_login
        font-size 10px
        color #fff
        position absolute
        left 138px
        top 28px
        transform translateY(-50%)
        .header_login_text
          color #fff
      .header_input
        position absolute
        left 15px
        top 55px
        input
          width 346px
          height 35px
          line-height 35px
          text-align center
          font-size 15px
          color #999999
      .header_inlog
        position absolute
        left 78px
        top 64px
        .el-icon-search
          font-size 16px
          color #999999
    .msite_nav
      bottom-border-1px(#e4e4e4)
      margin-top 100px
      height 200px
      background #fff
      .swiper-container
        width 100%
        height 100%
        .swiper-wrapper
          width 100%
          height 100%
          .swiper-slide
            display flex
            // justify-content center
            align-items flex-start
            flex-wrap wrap
            .link_to_food
              width 20%
              margin-top 12px 
              .food_container
                display block
                width 100%
                text-align center
                padding-bottom 10px
                font-size 0
                img
                  display inline-block
                  width 50px
                  height 50px
              span
                display block
                width 100%
                text-align center
                font-size 13px
                color #666
        .swiper-pagination
          >span.swiper-pagination-bullet-active
            background #02a774
    .Set_meal
      background-color #fff
      // margin-bottom 10px   
      .index-3xB2N_0
        padding 0px 10px
        width 355px
        height 185px
        .index-Q3GS5_0_index-1xT5J
          margin-bottom 5px
          border-radius 5px
          height 110px
          position relative
          background linear-gradient(0deg,#f4f4f4 5%,#fafafa 95%)
          padding 10px 0 0 10px
          .index-1qvN6_0
            font-size 17px
            color #000
            font-weight 700
            margin-bottom 5px
          .index-2W67h_0
            font-size 14px
            color #777
            margin-bottom 10px
          .index-1DFa7_0
            font-size 12px
            color #af8260
            font-weight 700
          .img
            width 140px
            height 90px
            position absolute
            right 18px
            top 15px
        .index-3eoZ-_0
          padding 0 5px 0 10px
          height 40px
          line-height 35px
          background-image linear-gradient(90deg,#ffefc4,#f3dda0)
          border-radius 2px
          .king
            width 20px
            height 20px
            margin-top 5px
          .index-M9mXY_0
            font-size 16px
            font-weight bold
          .index-tO6Fz_0
            font-size 12px
            color #644f1b
          .going
            font-size 12px
            margin-left 90px
            color #644f1b
    .msite_shop_list
      // top-border-1px(#e4e4e4)
      // margin-top 10px
      background #fff
      .shop_header
        padding 0px 10px 0
        text-align center
        .shop_icon
          margin-left 5px
          color #999
        .shop_header_title
          color #000
          font-size 16px
          line-height 20px
      .shop_search
        width 100%
        height 35px
        line-height 35px
        .ul_search
          &::befor
            conent ''
            display block
            clear both
          .li_search
            float left
            width 93px
            text-align center
            color #666666
            font-size 14px
            position relative
            .el-icon-caret-bottom
              color #666666
              position absolute
              top 11px
              left 76px
              font-size 10px
            .el-icon-table-lamp
              color #666666
              position absolute
              top 11px
              left 65px
</style>