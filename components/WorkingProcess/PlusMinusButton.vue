<script setup>
defineProps({
  isPlus: Boolean,
  size: Number,
});
</script>

<template>
  <!-- плюс -->
  <svg
    v-if="isPlus"
    :width="size"
    :height="size"
    viewBox="0 0 58 59"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <circle cx="29" cy="29.5" r="28.5" fill="#F3F3F3" stroke="#191A23" />
    <path
      d="M25.6 41.58V31.86H16V26.22H25.6V16.5H31.48V26.22H41.08V31.86H31.48V41.58H25.6Z"
      fill="#191A23"
    />
  </svg>

  <!-- минус -->
  <svg
    v-else
    width="58"
    height="59"
    viewBox="0 0 58 59"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <circle cx="29" cy="29.5" r="28.5" fill="#F3F3F3" stroke="#191A23" />
    <path d="M20 32.14V26.5H37.76V32.14H20Z" fill="black" />
  </svg>
</template>
