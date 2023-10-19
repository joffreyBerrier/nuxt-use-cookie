<script setup>
const { data, pending, error, refresh } = await useAsyncData(async() => {
  const test = await $fetch('https://jsonplaceholder.typicode.com/todos/1')

  const theme = useCookie('theme')
  theme.value = 'dark'

  return {
    test
  }
})

console.log('error', error.value)
</script>

<template>
  <div>
    {{ data }}
  </div>
</template>
