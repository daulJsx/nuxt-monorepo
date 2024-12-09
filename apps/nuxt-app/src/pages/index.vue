<template>
  <NxWelcome title="nuxt-app" />
  <MyButton @click="handleClick">Click Me</MyButton>
</template>

<script setup>
import { MyButton } from '@nuxt-monorepo/ui';

function handleClick() {
  alert('Button Clicked!');
}
</script>
