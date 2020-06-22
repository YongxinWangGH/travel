<template>
  <div class="wrapper">
    <swiper :options="swiperOption" >
      <swiper-slide  >
        <img class="swiper-img" src="https://secure.kimberleyquest.com.au/images/booking-engine-hero.jpg" />
      </swiper-slide>
      <swiper-slide  >
        <img class="swiper-img" src="https://kimberleyquest.com.au/wp-content/uploads/2019/03/hero-home.jpg" />
      </swiper-slide>
      <div class="swiper-pagination"  slot="pagination"></div>
    </swiper>
  </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  props: {
    list: Array
  },
  data () {
    return {
      swiperOption: {
        pagination: '.swiper-pagination',
        loop: true
      }
    }
  },
  computed: {
    
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background: #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
    background: #eee
    .swiper-img
      width: 100%
  .wrapper >>> .swiper-container
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 31.25%
</style>
