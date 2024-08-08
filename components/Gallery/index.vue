<script setup>
import { galleryData } from "./galleryData";

const currentSlide = ref(0);
</script>

<template>
  <div class="gallery container">
    <div class="gallery_mainframe">
      <img :src="galleryData[currentSlide].lg" alt="Большое изображение" />
    </div>
    <div class="gallery_picker">
      <img
        v-for="(item, index) in galleryData"
        :src="item.sm"
        @click="currentSlide = index"
        alt="Маленькое изображение"
      />
    </div>
  </div>
</template>

<style lang="scss"></style>
