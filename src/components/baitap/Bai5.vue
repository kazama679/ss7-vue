<script setup>
const emit = defineEmits(['messageSent'])
const props = defineProps(['titleProp', 'contentProp'])
</script>

<template>
  <div>
    <div class="display">
      <p>{{props.titleProp}}</p>
      <p>{{props.contentProp}}</p>
      <button @click="$emit('messageSent', false)">Close</button>
    </div>
  </div>
</template>

<style>
</style>