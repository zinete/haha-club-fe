<script setup lang="ts">

</script>

<template>
  <div>
    <div>
      <div class="flex flex-row">
        <div class="w-70% py-4">
          <div class="w-full bg-gray-1 dark:bg-gray-9 rounded-sm">
            <router-link
              v-for="item in 15" :key="item"
              :to="`/post/${item}`"
              class="p-4 border-b-1 dark:border-color-gray-8 dark-hover:bg-gray-5 hover:bg-gray-2 transition-color flex flex-row items-center"
            >
              <router-link :to="`/user/${item}`">
                <img
                  width="40"
                  height="40"
                  class="rounded-full"
                  src="https://img.w2solo.com/user/avatar/4089/1e0553.jpg?imageView2/3/w/96/h/96/q/100"
                >
              </router-link>
              <div class="ml-2 w-full flex flex-row items-center justify-between">
                <div>
                  <p class="text-base mb-2 opacity-80">
                    <strong class="text-red">最新</strong> 我的作品 为了帮你养成更健康的饮食习惯，我开发了这款 App——「杂食记」
                  </p>
                  <p class="text-sm opacity-50">
                    <strong class="text-gray-4">周杰伦 *</strong> 我的作品 为了帮你养成更健康的饮食习惯，我开发了这款 App——「杂食记」
                  </p>
                </div>
                <div>
                  <div class="px-2 rounded-xl bg-gray-6 block">
                    <span class="font-bold text-sm ">2</span>
                  </div>
                </div>
              </div>
            </router-link>
          </div>
        </div>
        <div class="w-30% py-4 ml-2">
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
