<template>
  <div class="form-control">
    <label v-if="label" class="label">
      <span class="label-text">{{ label }}</span>
      <a v-if="labelTopRight" href="#" class="label-text-alt">
        {{ labelTopRight }}
      </a>
    </label>
    <input
      v-model="datamodel"
      type="text"
      :placeholder="placeholder"
      class="input input-md input-primary"
    />
    <label v-if="labelBottomleft || labelBottomRight" class="label">
      <a v-if="labelBottomleft" href="#" class="label-text-alt">{{
        labelBottomleft
      }}</a>
      <a v-if="labelBottomRight" href="#" class="label-text-alt">{{
        labelBottomRight
      }}</a>
    </label>
  </div>
</template>
<script>
export default {
  props: {
    value: { type: String, default: null },
    label: { type: String, default: null },
    placeholder: { type: String, default: null },
    labelTopRight: { type: String, default: null },
    labelBottomRight: { type: String, default: null },
    labelBottomleft: { type: String, default: null }
  },
  computed: {
    datamodel: {
      get() {
        return this.value
      },
      set(val) {
        this.$emit('input', val)
      },
    },
  },
}
</script>
