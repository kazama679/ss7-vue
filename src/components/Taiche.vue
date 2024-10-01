<script setup>
const props = defineProps({
    title: {
        default: "click mặc định",
        type: String,
        required: false // bắt buộc p truyền vào nếu là false
    }
})
</script>

<template>
  <div>
    <button>
      <slot></slot>
    </button>
  </div>
</template>

<style>

</style>