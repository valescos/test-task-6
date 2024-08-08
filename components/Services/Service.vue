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
    <div>
      <div>
        <h3>{{ firstline }}</h3>
        <h3>{{ secondline }}</h3>
      </div>
      <button><ArrowIcon /> Learn More</button>
    </div>
    <img :src="img" alt="Иллюстрация" />
  </div>
</template>

<style lang="scss"></style>
