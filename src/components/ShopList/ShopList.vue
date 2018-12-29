<template>
  <div class="shop_container">
    <ul class="shop_list">
      <li class="shop_li">
        <a>
          <div class="shop_left">
            <img src="../../pages/Msite/images/shop/1.jpg" alt="" class="shop_img">
          </div>
          <div class="shop_right">
            <section class="shop_detail_header">
              <span class="shop_detail_header_left">
                <span class="shop_detail_lable">
                  品牌
                </span>
                <span class="shop_detail_title">
                  大闸蟹
                </span>
              </span>
              <ul class="shop_detail_ul">
                <li class="supports">1</li>
              </ul>
            </section>
            <section class="shop_rating_order">
              <div class="shop_rating_order_left">
                <div class="star">xxx</div>
                <div class="rating_section">4.5</div>
                <div class="order_section">月售1单</div>
              </div>
              <div class="shop_rating_order_right">
                <span class="delivery_style">配送</span>
              </div>
            </section>
            <section class="shop_distance">
              <p class="shop_delivery_msg">
                <span>$100元起送</span>
                <span class="segmentation">/</span>
                <span>配送费约10元</span>
              </p>
            </section>
          </div>
        </a>
      </li>

    </ul>
  </div>
</template>

<script>
  export default {
    name: "ShopList"
  }
</script>

<style scoped lang='stylus' rel='stylesheet/stylus'>
  .shop_container

    width 100%
    background #fff
    .shop_list
      .shop_li
        padding 12px 8px
        bottom-border-1px(#f1f1f1)
        > a
          display flex
          justify-content space-between
          .shop_left
            width 22%
            .shop_img
              display block
              width 100%
              /*height 100%*/
          .shop_right
            width 78%
            .shop_detail_header
              display flex
              justify-content space-between
              width 100%
              .shop_detail_header_left
                font-size 0
                .shop_detail_lable
                  font-size 12px
                  background #ffd930
                  padding 1px 2px
                  text-align center
                  border-radius 2px
                  color #333
                  margin-right 4px
                .shop_detail_title
                  font-size 16px
                  color: #333
                  display inline-block
                  width 120px
                  overflow hidden
                  white-space nowrap
                  -ms-text-overflow: ellipsis
                  text-overflow: ellipsis
                  position relative
                  top: 2px
                  font-weight 700

            .shop_rating_order
              margin: 20px 0 14px
              display flex
              justify-content space-between
              .shop_rating_order_left
                display flex
                color #ff9a0d
                font-size 10px
                font-weight 700
                .rating_section
                  font-size 10px
                  color #ff6000
                  margin: 0 4px
                .order_section
                  font-size 10px
                  color #666
              .shop_rating_order_right
                font-size 12px
                color #666
            .shop_distance
              .shop_delivery_msg
                font-size 12px
                color: #666
                .segmentation
                  color: #ccc
</style>
