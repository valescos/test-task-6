<script setup>
defineProps({
  title: String,
  text: String,
  index: Number,
});

const isOpen = ref(false);
</script>

<template>
  <div class="working_process_item">
    <div class="working_process_item_header">
      <div>
        <p>{{ "0" + (index + 1) }}</p>
        <h3>{{ title }}</h3>
      </div>
      <button @click="isOpen = !isOpen">+</button>
    </div>
    <p v-if="isOpen">{{ text }}</p>
  </div>
</template>

<style lang="scss"></style>
