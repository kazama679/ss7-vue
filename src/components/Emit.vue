<script setup>
const emit = defineEmits(['onClick']);

const handleClick=()=>{
    emit('onClick', 'xin chào các bạn')
}
</script>

<template>
  <div>
    <button @click="handleClick">
        <slot></slot>
    </button>
  </div>
</template>

<style>

</style>