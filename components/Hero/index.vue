<script setup>
import { heroData } from "./heroData";
</script>

<template>
  <div class="hero">
    <div>
      <h1>{{ heroData.title }}</h1>
      <p>{{ heroData.text }}</p>
      <button>{{ heroData.button.text }}</button>
    </div>
    <img :src="heroData.img" alt="Иллюстрация" />
  </div>
</template>

<style lang="scss"></style>
