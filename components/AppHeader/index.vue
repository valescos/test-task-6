<script setup>
import { headerData } from "./headerData";
import HeaderMenu from "./HeaderMenu.vue";

const isMenuOpened = ref(false);
</script>

<template>
  <header class="header container">
    <Logo :size="36" variant="black" class="logo" />
    <Logo :size="26" variant="black" class="small_logo" />
    <div>
      <Navigation variant="black" class="header_nav" />
      <button class="btn">{{ headerData.button.text }}</button>
      <button @click="isMenuOpened = !isMenuOpened" class="burger">
        <img :src="headerData.burger" />
      </button>
    </div>
    <HeaderMenu v-if="isMenuOpened" class="header_menu" />
  </header>
</template>

<style lang="scss"></style>
