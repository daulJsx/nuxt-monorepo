<template>
  <button class="btn" @click="handleClick">
    <slot></slot>
  </button>
</template>

<script setup>
defineProps({
  onClick: Function,
});

function handleClick() {
  if (typeof onClick === 'function') {
    onClick();
  }
}
</script>

<style scoped>
.btn {
  padding: 8px 16px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 4px;
}
</style>
