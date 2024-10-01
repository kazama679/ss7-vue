<script setup>
// const props = defineProps(['conName2', 'ageProps'])
// cách dùng di tras tơ ring
// const { name, age } = defineProps(['conName2', 'ageProps'])

const props = defineProps(['arr1'])
</script>

<template>
  <div>Con
    <!-- <p>tên: {{props.conName2}}</p> -->
    <!-- <p>tên: {{name}}</p> -->
    <!-- <p>tuổi: {{props.ageProps}}</p>  -->
    <!-- <p>tuổi: {{age}}</p>  -->
    <p>{{props.arr1.name}}</p>
    <p>{{props.arr1.id}}</p>
    <p>{{props.arr1.age}}</p>
  </div>
</template>

<style>

</style>