<script setup>
defineProps({
  title: String,
  img: String,
});
</script>

<template>
  <div class="service">
    <div>
      <h3>{{ title }}</h3>
      <button>Learn More</button>
    </div>
    <img :src="img" alt="Иллюстрация" />
  </div>
</template>

<style lang="scss"></style>
