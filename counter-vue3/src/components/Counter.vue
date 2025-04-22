<script setup lang="ts">
import { ref } from "vue";
const count = ref(0);
const addingOne = () => {
  count.value++;
};
const resetNum = () => {
  count.value = 0;
};
</script>

<template>
  <h1>{{ count }}</h1>
  <button @click="addingOne">+1</button>
  <button @click="resetNum">Reset</button>
</template>
