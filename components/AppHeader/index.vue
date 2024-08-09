<script setup>
import { headerData } from "./headerData";
</script>

<template>
  <header class="header container">
    <Logo :size="36" variant="black" class="logo" />
    <Logo :size="26" variant="black" class="small_logo" />
    <div>
      <Navigation variant="black" class="header_nav" />
      <button class="btn">{{ headerData.button.text }}</button>
      <button class="burger"><img :src="headerData.burger" /></button>
    </div>
  </header>
</template>

<style lang="scss"></style>
