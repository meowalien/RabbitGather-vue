<script setup lang="ts">

defineProps<{
  list: {
    name: string
    path: string
  }[]
}>()


</script>

<template>
  <div class="flex flex-col items-center justify-start">
    <ul class="w-full flex flex-row flex-wrap justify-around">
      <li class="m-1 text-sm border-red-500" v-for="item in list" >
        <img class="inline align-baseline h-5 transform -rotate-30 mx-1" src="/carrot.svg" alt="RabbitGather logo" />
        <a :href="item.path">
          {{item.name}}
        </a>
      </li>
    </ul>
  </div>
</template>

<style scoped>
</style>
