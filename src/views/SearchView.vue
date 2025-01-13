<template>
   <HeaderComponent />
   <div>
      <h1>Search</h1>
   </div>
   <div class="search">
      <input v-model="searchInput" type="text">
      <button @click="cl" class="search-button">Найти</button>
   </div>
   <div class="result">
      <h2>{{ result }}</h2>
   </div>
</template>

<script setup lang="ts">
import HeaderComponent from '@/components/HeaderComponent.vue';
import { ref } from 'vue';

const searchInput = ref("")
const result = ref()
const arr1 = [1,2,3,4,5,6,7]
const cl = () => {
   arr1.includes(+searchInput.value) ? result.value = +searchInput.value : result.value = "не найдено"
   console.log(searchInput.value)
}


</script>

<style scoped>
h1 {
   text-align: center;
}
.search {
   display: flex;
   justify-content: center;
   gap: 20px;
}
</style>