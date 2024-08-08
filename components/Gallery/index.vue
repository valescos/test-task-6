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
      <div
        v-for="(item, index) in galleryData"
        :key="index"
        class="gallery_picker_item"
        :class="currentSlide === index && 'gallery_picker_item_selected'"
      >
        <img
          :src="item.sm"
          @click="currentSlide = index"
          alt="Маленькое изображение"
        />
      </div>
    </div>
  </div>
</template>

<style lang="scss"></style>
