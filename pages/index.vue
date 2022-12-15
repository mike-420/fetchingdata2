<template>
    <ul>
      <li v-for="shop in shops" :key="shop.id">
        {{ shop.name }}
      </li>
    </ul>
</template>
<script setup>
  const { data : shops } = await useFetch('https://mocki.io/v1/3fa1924f-6c6b-4d49-b9ec-d91f6da13c3c')
</script>

