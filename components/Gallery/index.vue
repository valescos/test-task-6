<script setup>
import { galleryData } from "./galleryData";

const currenSlide = ref(0);
</script>

<template>
  <div class="gallery container">
    <Swiper
      :modules="[SwiperPagination]"
      :slides-per-view="1"
      :loop="true"
      :pagination="{
        clickable: true,
      }"
      class="swiper-container"
    >
      <SwiperSlide v-for="slide in galleryData.map((i) => i.lg)" :key="slide">
        <img :src="slide" class="slide" />
      </SwiperSlide>
    </Swiper>
  </div>
</template>

<style lang="scss">
.swiper-pagination-bullet-active {
  background-color: #191a23;
}
</style>
