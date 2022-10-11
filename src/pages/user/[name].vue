<script setup lang="ts">
const props = defineProps<{ name: any }>()
</script>

<template>
  <div>
    <div>
      <div class="flex flex-row pt-2 pb-10">
        <div class="w-70% ">
          <div class="w-full bg-gray-1 dark:bg-gray-9 rounded-sm p-4">
            <h2 class="text-gray-4 text-2xl font-bold mb-2">
              {{ props.name }}
            </h2>
            lll {{ props }}
          </div>
        </div>
        <div class="w-30%  ml-2">
          <div class="w-full p-4 bg-gray-1 dark:bg-gray-9 rounded-sm">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic, deleniti! Alias dignissimos dolorem itaque cum ea enim impedit, tempore vel harum provident aliquam ipsum in debitis ullam corrupti repudiandae aperiam!
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
