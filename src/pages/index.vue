<script setup lang="ts">

</script>

<template>
  <div>
    <div>
      <div class="flex md:flex-row flex-col pt-2 pb-10">
        <div class="w-full md:w-70%">
          <div class="w-full bg-gray-1 dark:bg-gray-9 rounded-sm">
            <div v-for="item in 10" :key="item">
              <post-item :post="item" />
            </div>
          </div>
        </div>
        <div class="md:w-30% w-full md:ml-2">
          <div class="w-full p-4 bg-gray-1 dark:bg-gray-9 rounded-sm">
            <div class="btn w-full bg-green-9 dark:bg-green-6 opacity-80 h-12 flex justify-center items-center">
              发布新的哈哈
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
