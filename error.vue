<template>
  <template v-if="error.statusCode === 404 || '404'">
    <p>[template]: Oops page not available 🥺</p>
  </template>
</template>

<script setup>
const props = defineProps({
  error: Object,
});
</script>
