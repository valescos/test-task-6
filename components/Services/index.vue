<script setup>
import { servicesData } from "./servicesData";
import Service from "./Service.vue";
</script>

<template>
  <section class="services container">
    <div class="services_header">
      <h2>{{ servicesData.title }}</h2>
      <p>{{ servicesData.text }}</p>
    </div>
    <div class="services_wrapper">
      <Service
        v-for="item in servicesData.list"
        :title="item.title"
        :img="item.img"
      />
    </div>
  </section>
</template>

<style lang="scss"></style>
