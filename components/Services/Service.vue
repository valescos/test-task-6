<script setup>
import ArrowIcon from "./ArrowIcon.vue";

defineProps({
  firstline: String,
  secondline: String,
  img: String,
  index: Number,
});
</script>

<template>
  <div
    class="service"
    :class="
      [1, 4].includes(index)
        ? 'service-green'
        : index === 2
        ? 'service-black'
        : index === 5
        ? 'service-black last'
        : null
    "
  >
    <div class="service_header">
      <h3>{{ firstline }}</h3>
      <h3>{{ secondline }}</h3>
    </div>
    <div class="service_content">
      <button><ArrowIcon /><span>Learn More</span></button>
      <img :src="img" alt="Иллюстрация" />
    </div>
  </div>
</template>

<style lang="scss"></style>
