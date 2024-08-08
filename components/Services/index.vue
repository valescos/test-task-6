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
    <div class="services_content">
      <Service
        v-for="(item, index) in servicesData.list"
        :key="index"
        :firstline="item.firstline"
        :secondline="item.secondline"
        :img="item.img"
        :index="index"
      />
    </div>
  </section>
</template>

<style lang="scss"></style>
