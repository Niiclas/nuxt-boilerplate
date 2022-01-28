<template>
  <div :class="{ 'col-span-2': full }">
    <slot />
  </div>
</template>
<script>
export default {
  props: {
    full: Boolean,
  },
}
</script>
