<script setup>
import { headerData } from "./headerData";
</script>

<template>
  <div class="header">
    <Logo :size="36" variant="black" />
    <div>
      <Navigation variant="black" />
      <button>{{ headerData.button.text }}</button>
      <button><img :src="headerData.burger" /></button>
    </div>
  </div>
</template>

<style lang="scss"></style>
