<script setup>
import { headerData } from "./headerData";
</script>

<template>
  <header class="header container">
    <Logo :size="36" variant="black" />
    <div>
      <Navigation variant="black" />
      <button class="btn">{{ headerData.button.text }}</button>
      <button class="burger"><img :src="headerData.burger" /></button>
    </div>
  </header>
</template>

<style lang="scss"></style>
