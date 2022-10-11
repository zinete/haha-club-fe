<script setup lang="ts">
const postItem = defineProps<{ post: any }>()

const commit = (num: number) => {
  if (num > 99)
    return '99+'
  else
    return num
}
</script>

<template>
  <div>
    <div

      class="p-4 border-b-1 dark:border-color-gray-8 dark-hover:bg-gray-7 hover:bg-gray-2 transition-color flex flex-row"
    >
      <router-link :to="`/user/${postItem.post}`">
        <img
          width="48"
          height="48"
          class="rounded-lg"
          src="https://www.zinete.com/images/p2.jpg"
        >
      </router-link>
      <div class="ml-4 w-full flex flex-row md:items-center justify-between">
        <div>
          <div class="flex flex-row items-center mb-1 ">
            <!-- <strong class="text-red-4">最新</strong> -->
            <router-link
              :to="`/post/${postItem.post}`"
              class="text-base block opacity-90 hover:underline"
            >
              我的作品 为了帮你养成更健康的饮食习惯，我开发了这款 App——「杂食记」
              我的作品 为了帮你养成更健康的饮食习惯，我开发了这款 App——「杂食记」
              我的作品 为了帮你养成更健康的饮食习惯，我开发了这款 App——「杂食记」
            </router-link>
          </div>

          <div class="text-sm opacity-50 flex-row flex items-center">
            <tag class="bg-gray-6 block px-1 rounded-sm text-[10px] text-white">
              便签
            </tag>
            <strong class="text-gray-4 mx-2">周杰伦</strong>

            <time class="mr-2">4天前</time>
            <p>
              最后回复来自<strong class="text-gray-1">渣渣辉</strong>
            </p>
          </div>
        </div>
        <div class="ml-6">
          <div class="px-2 h-5 rounded-full flex flex-row items-center justify-center bg-gray-3 dark:bg-gray-6">
            <span class="font-bold text-[10px]">{{
              commit(postItem.post + 95)
            }}</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
