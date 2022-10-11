<script setup lang="ts">
// const { t, availableLocales, locale } = useI18n()

const getNowCopyRight = () => {
  return `CopyRight@${new Date().getFullYear()} · HAHA-CLUB`
}
// const toggleLocales = () => {
//   // change to some real logic
//   const locales = availableLocales
//   locale.value = locales[(locales.indexOf(locale.value) + 1) % locales.length]
// }
</script>

<template>
  <footer class="bg-gray-1 dark:bg-gray-9 h-30">
    <div class="flex h-full justify-center items-center">
      <span class="opacity-60 text-sm">{{ getNowCopyRight() }}</span>
    </div>
  </footer>
</template>
