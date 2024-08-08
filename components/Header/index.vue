<script setup>
import { headerData } from "./headerData";
</script>

<template>
  <div class="header">
    <img :src="headerData.logo" alt="Логотип" />
    <div>
      <ul>
        <li v-for="item in headerData.navigation" :key="item">{{ item }}</li>
      </ul>
      <button>{{ headerData.button.text }}</button>
      <button><img :src="headerData.burger" /></button>
    </div>
  </div>
</template>

<style lang="scss"></style>
