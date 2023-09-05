<script setup lang="ts">
import Logo from '@/components/Logo.vue'
import ComponentList from '@/components/ComponentList.vue'
import {ref} from 'vue'


const listMock = ref(
    [{name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }, {name: "Web Monitoring Crawler", path: "/web-monitoring-crawler"}, {
      name: "Web Monitoring Crawler",
      path: "/web-monitoring-crawler"
    }]
)

</script>

<template>
  <div class="w-full h-full flex flex-col items-center justify-start ">
    <div class="w-4/5 flex flex-col ">
      <Logo class="w-full"></Logo>
      <ComponentList class="w-full min-h-20" :list="listMock"></ComponentList>
    </div>
  </div>
</template>

<style scoped>

</style>
