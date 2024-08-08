<script setup>
import PlusMinusButton from "./PlusMinusButton.vue";
defineProps({
  title: String,
  text: String,
  index: Number,
});

const isOpen = ref(false);
</script>

<template>
  <div class="working_process_item" :class="isOpen && 'opened'">
    <div class="working_process_item_header">
      <div>
        <h1>{{ "0" + (index + 1) }}</h1>
        <h3>{{ title }}</h3>
      </div>
      <button @click="isOpen = !isOpen">
        <PlusMinusButton :isPlus="!isOpen" :size="58" />
      </button>
    </div>
    <div v-if="isOpen" class="working_process_item_body">
      <hr />
      <p>{{ text }}</p>
    </div>
  </div>
</template>

<style lang="scss"></style>
