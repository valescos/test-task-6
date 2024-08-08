<script setup>
import { workingProcessData } from "./workingProcessData";
import WorkingProcessItem from "./WorkingProcessItem.vue";
</script>

<template>
  <div class="working_process">
    <div class="working_process_header">
      <h2>{{ workingProcessData.title }}</h2>
      <p>{{ workingProcessData.text }}</p>
    </div>
    <div class="working_process_wrapper">
      <WorkingProcessItem
        v-for="(item, index) in workingProcessData.list"
        :key="index"
        :index="index"
        :title="item.title"
        :text="item.text"
      />
    </div>
  </div>
</template>

<style lang="scss"></style>
