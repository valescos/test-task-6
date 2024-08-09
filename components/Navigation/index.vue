<script setup>
import { navigationData } from "./navigationData";
</script>

<template>
  <nav class="navigation">
    <ul>
      <li v-for="item in navigationData" :key="item">{{ item }}</li>
    </ul>
  </nav>
</template>
