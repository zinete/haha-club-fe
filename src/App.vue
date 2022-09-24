<script setup lang="ts">
// https://github.com/vueuse/head
// you can use this to manipulate the document head in any components,
// they will be rendered correctly in the html results with vite-ssg
useHead({
  title: 'HaHa-CLUB',
  meta: [
    { name: 'description', content: 'ha ha ha ha ha ha ....' },
    {
      name: 'theme-color',
      content: computed(() => isDark.value ? 'text-blue' : 'text-white'),
    },
  ],
  link: [
    {
      rel: 'icon',
      type: 'image/svg+xml',
      href: computed(() => preferredDark.value ? '/favicon-dark.svg' : '/favicon.svg'),
    },
  ],
})
</script>

<template>
  <RouterView />
</template>
