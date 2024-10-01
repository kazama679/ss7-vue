<script setup>
const props = defineProps(['Childen'])
</script>

<template>
  <div>Bai2
    <p>{{props.Childen.id}}</p>
    <p>{{props.Childen.name}}</p>
    <p>{{props.Childen.price}}</p>
    <p>{{props.Childen.quantity}}</p>
  </div>
</template>

<style>

</style>