<template>
  <div class="text-base-300 flex flex-col items-center">
    <h2 class="text-center text-7xl">Huhu! Ich bin {{ name }}</h2>
    <div class="mt-12 flex flex-row justify-center items-center">
      <div class="mr-3">Nicht {{ name }}?</div>
      <m-input v-model="name" />
    </div>
    <NuxtLink class="mt-2 text-xs" to="/ueber_uns/geschichte"
      >Hier eine andere Seite</NuxtLink
    >
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      name: 'Kevin',
    }
  },
}
</script>
