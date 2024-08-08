<script setup>
import { clientsData } from "./clientsData";
</script>

<template>
  <section class="clients container">
    <div v-for="item in clientsData">
      <img :src="item" alt="Логотип компании" />
    </div>
  </section>
</template>

<style lang="scss"></style>
