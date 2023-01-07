<script setup>
const { data } = await useAsyncData("home", () => queryContent("/").findOne());
</script>

<template>
  <section id="intro">
    <h1 class="text-3xl font-bold underline">This is a course page</h1>
    <div class="bg-red-100 py-9">
      <NuxtPage></NuxtPage>
    </div>
    <pre>    {{ data }}  </pre>
  </section>
</template>
