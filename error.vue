<template>
  <template v-if="error.statusCode === 404 || '404'">
    <p>[template]: Oops page not available 🥺</p>
  </template>
</template>

<script setup>
const props = defineProps({
  error: Object,
});
const error = useError();
if (error.value.statusCode === 404 || "404") {
  error.value.message = "[script]: Oops! Page not found 😔";
}
</script>
