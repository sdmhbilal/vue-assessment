<template>
  <div>
    <VueMultiselect
      v-model="selected"
      :multiple="true"
      :options="options"
      label="label"
      track-by="value"
    >
    </VueMultiselect>
  </div>
</template>

<script>
import VueMultiselect from 'vue-multiselect'

export default {
  components: { VueMultiselect },
  watch: {
    selectedOptions() {
      this.$emit('update', this.selected)
    }
  },
  props: {
    options: {
      type: Array,
      required: true
    }
  },
  data () {
    return {
      selected: null
    }
  }
}
</script>

<style src="vue-multiselect/dist/vue-multiselect.css"></style>
