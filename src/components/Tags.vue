<script setup lang="ts">
import { ref } from 'vue'
const tag = ref([
  {
    name: '最热',
    path: '/hots',
  },
  {
    name: '音乐',
    path: '/music',
  },
  {
    name: '游戏',
    path: '/games',
  },
  {
    name: '电影',
    path: '/movies',
  },
  {
    name: '哈哈',
    path: '/haha',
  },
])

const router = useRouter()
</script>

<template>
  <div>
    <div class="flex flex-row h-10 border-b-gray-300 dark:border-color-gray-8 border-b-0.5 w-full items-center px-10% 2xl:px-15%">
      <div
        v-for="item in tag"
        :key="item.name" :class="router.currentRoute.value.fullPath === item.path ? 'text-blue' : ''"
        class="mr-5 font-400 text-base opacity-80"
      >
        <router-link :to="item.path">
          {{ item.name }}
        </router-link>
      </div>
    </div>
  </div>
</template>

  <style scoped>

  </style>

