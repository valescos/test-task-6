<script setup>
import { headerData } from "./headerData";
</script>

<template>
  <header class="header container">
    <Logo :size="36" variant="black" />
    <div>
      <Navigation variant="black" />
      <button>{{ headerData.button.text }}</button>
      <button><img :src="headerData.burger" /></button>
    </div>
  </header>
</template>

<style lang="scss"></style>
