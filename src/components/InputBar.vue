<script setup lang="ts">

const { name, modelValue } = defineProps(['name', 'modelValue']);
const emit = defineEmits(['update:modelValue']);

const updateMessage = (value: Event) => {
  const inputValue = (value.target as HTMLInputElement).value;
  emit('update:modelValue', inputValue);
};

</script>

<template>
  <div class="flex flex-row items-center">
    <span class="align-baseline">{{name}}:&nbsp;&nbsp;</span>
    <input class="flex-1 bg-black border-b-1 focus:outline-none" :value="modelValue" @input="updateMessage">
  </div>
</template>
