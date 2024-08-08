<script setup>
import { workingProcessData } from "./workingProcessData";
import WorkingProcessItem from "./WorkingProcessItem.vue";
</script>

<template>
  <section class="working_process container">
    <div class="working_process_header">
      <h2>{{ workingProcessData.title }}</h2>
      <p>{{ workingProcessData.text }}</p>
    </div>
    <div class="working_process_content">
      <WorkingProcessItem
        v-for="(item, index) in workingProcessData.list"
        :key="index"
        :index="index"
        :title="item.title"
        :text="item.text"
      />
    </div>
  </section>
</template>

<style lang="scss"></style>
