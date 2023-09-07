<script setup lang="ts">
import InputBar from "@/components/InputBar.vue";
import { ref } from 'vue';

// Factory function for input fields
const createInputFields = () => [
  { name: "Name", fieldValue: ref("") },
  { name: "URL", fieldValue: ref("") },
  { name: "Selector", fieldValue: ref("") },
  { name: "Check interval", fieldValue: ref("") },
  { name: "Trigger event", fieldValue: ref("") },
  { name: "Notify to", fieldValue: ref("") }
];

const inputFields = createInputFields();
</script>
<template>
  <div class="w-full h-full  border-blue-500 flex flex-col items-center justify-start">
    <div class="pt-10 max-w-1/2 w-90 flex flex-col items-start justify-start">
      <InputBar class="w-full" v-for="inputField in inputFields" :key="inputField.name" :name="inputField.name" v-model="inputField.fieldValue.value"></InputBar>
    </div>
  </div>

</template>

<style scoped>

</style>
