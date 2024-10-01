<script setup>
const emit = defineEmits(['messageSent'])
</script>

<template>
  <div>
      <button @click="$emit('messageSent')">Tăng 1</button>
  </div>
</template>

<style>

</style>