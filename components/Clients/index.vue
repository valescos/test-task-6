<script setup>
import { clientsData } from "./clientsData";
</script>

<template>
  <div class="clients">
    <div v-for="item in clientsData">
      <img :src="item" alt="Логотип компании" />
    </div>
  </div>
</template>

<style lang="scss"></style>
