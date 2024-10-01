<script setup>
const emit = defineEmits(['messageSent'])
</script>

<template>
  <div>
      <button @click="$emit('messageSent', 1)">Delete</button>
  </div>
</template>

<style>

</style>