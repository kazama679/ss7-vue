<script setup>
</script>

<template>
  <div class="card">
    <div class="card-header">
      <slot name="header"></slot>
    </div>
    <div class="card-body">
      <slot name="body"></slot>
    </div>
    <div class="card-footer">
      <slot name="footer"></slot>
    </div>
  </div>
</template>

<style scoped>
.card {
  border: 1px solid #ddd;
  padding: 1rem;
  border-radius: 0.5rem;
}

.card-header, .card-body, .card-footer {
  margin-bottom: 0.5rem;
}
</style>