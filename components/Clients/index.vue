<script setup>
import { clientsData } from "./clientsData";
</script>

<template>
  <section class="clients container">
    <div class="clients_full">
      <img v-for="item in clientsData" :src="item" alt="Логотип компании" />
    </div>
    <div class="clients_first_half">
      <img
        v-for="item in clientsData.slice(0, clientsData.length / 2)"
        :src="item"
        alt="Логотип компании"
      />
    </div>
    <div class="clients_second_half">
      <img
        v-for="item in clientsData.slice(clientsData.length / 2)"
        :src="item"
        alt="Логотип компании"
      />
    </div>
  </section>
</template>

<style lang="scss"></style>
