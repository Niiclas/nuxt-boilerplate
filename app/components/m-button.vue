<template>
  <button
    class="btn"
    :class="{ 'btn-primary': primary }"
    @click="$emit('click')"
  >
    <slot />
  </button>
</template>
<script>
export default {
  props: {
    primary: Boolean,
  },
}
</script>
