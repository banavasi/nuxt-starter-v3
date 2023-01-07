<template>
  <section id="intro">
    <h1 class="text-3xl font-bold underline">Lesson page</h1>
    <p>chapter {{ $route.params.chapterSlug }}</p>
    <p>lesson {{ $route.params.lessonSlug }}</p>
  </section>
</template>
