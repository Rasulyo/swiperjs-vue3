<template>
  <h1>The Best Anime Charachters!</h1>
  <swiper
    :effect="'cube'"
    :grabCursor="true"
    :cubeEffect="{
      shadow: true,
      slideShadows: true,
      shadowOffset: 200,
      shadowScale: 1.94,
    }"
    :pagination="true"
    :modules="modules"
    :navigation="true"
    class="mySwiper"
  >
    <swiper-slide
      ><img
        src="https://i.pinimg.com/originals/e5/fb/28/e5fb28416a52f5cbe09bce587bb6a9a6.jpg" />
        </swiper-slide
    ><swiper-slide
      ><img
        src="https://i.pinimg.com/originals/e9/e9/30/e9e93013cc127bb3fe7aa30358ca1872.png" /></swiper-slide
    ><swiper-slide
      ><img src="https://cdn.bhdw.net/im/itachi-uchiha-naruto-oboi-86192_w635.jpg"
    /></swiper-slide>
    <swiper-slide>
      <img src="https://avatarfiles.alphacoders.com/666/66616.jpg" />
    </swiper-slide>
  </swiper>
</template>
<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/navigation";
import "./assets/style.css";
import "swiper/css/effect-cube";
import { EffectCube, Navigation, Pagination } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Navigation, Pagination, EffectCube],
    };
  },
};
</script>

<style lang="scss"></style>
