<script setup lang="ts">
const router = useRouter()
// const { t, availableLocales, locale } = useI18n()
const { t } = useI18n()
// const toggleLocales = () => {
//   // change to some real logic
//   const locales = availableLocales
//   locale.value = locales[(locales.indexOf(locale.value) + 1) % locales.length]
// }
</script>

<template>
  <header class="border-b-1 dark:border-color-gray-8 h-12 flex flex-row items-center justify-between px-8%">
    <!-- <a class="icon-btn mx-2" :title="t('button.toggle_langs')" @click="toggleLocales()">
      <div i-carbon-language />
    </a> -->
    <div class="flex flex-row">
      <button class="text-xl text-pink-6 font-600 hover:text-pink-8" @click="router.replace('/')">
        HaHa Club
      </button>
      <button class="icon-btn mx-2 !outline-none" :title="t('button.toggle_dark')" @click="toggleDark()">
        <div i="carbon-sun dark:carbon-moon" />
      </button>
    </div>
    <div>
      <div>Login</div>
    </div>
  </header>
  <Tags />
</template>

<style scoped>

</style>
