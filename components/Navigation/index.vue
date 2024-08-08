<script setup>
import { navigationData } from "./navigationData";

defineProps({
  variant: String,
});
</script>

<template>
  <nav class="navigation">
    <ul :class="variant === black ? 'navigation_black' : 'navigation_white'">
      <li v-for="item in navigationData" :key="item">{{ item }}</li>
    </ul>
  </nav>
</template>
