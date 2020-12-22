<template>
  <header>
    <v-container>
      <v-row>
        <v-col cols="12" md="6">
          <div class="header_title">
            <h1>
              Mahsultongizni xaridorgir bo’lishini xohlaysizmi?
            </h1>
            <p>
              Unda darhol biz bilan bog’laning va o'z mahsulotiz uchun chiroyli,
              <br />
              zamonaviy dizayn va upakovkaga ega bo'ling. <br />
              Zamonaviy upakovkaga buyurtma bering!
            </p>
            <v-btn class="btnDep" tag="a" depressed color="#FEB11B">
              Buyurtma berish
            </v-btn>
          </div>
        </v-col>
        <v-col cols="12" md="6">
          <div class="swiper_wrapper">
            <swiper class="swiper" :options="swiperOption">
              <swiper-slide v-for="n in 6" :key="n">
                <img :src="require('../assets/images/swiper.jpg')" alt="" />
              </swiper-slide>
            </swiper>
            <div class="swiper-button-prev swiperPrev" slot="button-prev"></div>
            <div class="swiper-button-next swiperNext" slot="button-next"></div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </header>
</template>
<script>
import SwiperCore, { EffectCoverflow, Navigation, Autoplay } from "swiper";
SwiperCore.use([Navigation, EffectCoverflow, Autoplay]);
import { Swiper, SwiperSlide } from "vue-awesome-swiper";
import "swiper/swiper-bundle.min.css";
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      swiperOption: {
        effect: "coverflow",
        grabCursor: true,
        centeredSlides: true,
        loop: true,
        slidesPerView: "auto",
        autoplay: {
          delay: 4000,
        },
        coverflowEffect: {
          rotate: 0,
          stretch: 160,
          depth: 300,
          modifier: 1.5,
          slideShadows: false,
        },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
      },
    };
  },
};
</script>
<style lang="scss" scoped>
header{
  padding-bottom: 100px;
}
.header_title {
  padding-top: 140px;
}
.header_title h1 {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: bold;
  font-size: 48px;
  line-height: 65px;
  color: #000000;
}
.header_title p {
  font-family: "Open Sans", sans-serif;
  font-style: normal;
  font-weight: normal;
  font-size: 24px;
  line-height: 130%;
  /* or 31px */
  color: #000000;
  margin-top: 50px;
  margin-bottom: 50px;
}
.header_title .btnDep {
  padding: 23px 62px !important;
  height: auto !important;
  font-weight: 600 !important;
  font-size: 24px !important;
}
.swiper_wrapper {
  padding-top: 88px;
  position: relative;
  padding-bottom: 40px;
  .swiperPrev{
    z-index: 3;
    top: 100%;
    left: 113px;
    &::after{
      content: url('../assets/images/prev.png');
      font-size: 0px;
    }
  }
  .swiperNext{
    z-index: 3;
    left: 175px;
    right: auto;
    top: 100%;
    &::after{
      content: url('../assets/images/next.svg');
      font-size: 0px;
    }
  }
}
.swiper_wrapper::after {
  content: "";
  display: block;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  background: white;
  z-index: 2;
  width: 106px;
}
.swiper {
  height: 100%;
  width: 100%;

  .swiper-slide {
    display: flex;
    justify-content: center;
    align-items: center;
    width: auto;
    height: auto;
    text-align: center;
    font-weight: bold;
    // font-size: $font-size-huge * 2;
    background-color: #2c8dfb;
    background-position: center;
    background-size: cover;
    color: white;
    img {
      max-width: 100%;
      height: auto;
    }
  }
}
@media (max-width:1904px) {
  .swiper_wrapper::after {
    display: none;
  }
}
</style>
