<script setup lang="ts">
const router = useRouter()
</script>

<template>
  <div class="flex justify-center items-center py-20">
    <div class="flex flex-col text-center">
      <span class="text-2xl font-500 text-red-5 mb-2"> 404 Not Find </span>
      <p>来到了一个不存在的地方</p>
      <p class="btn mt-4 block" @click="router.back()">
        back
      </p>
    </div>
  </div>
</template>

<style scoped>

</style>
