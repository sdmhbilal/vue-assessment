<template>
  <div>
    <MultiSelect
      :options="selectOptions"
      :selectedValues="selectedValues"
      @update="onUpdate($event)"
    />
  </div>
</template>

<script>
import MultiSelect from './DropDown.vue';

export default {
  components: {
    MultiSelect
  },
  data() {
    return {
      selectOptions: [
        { label: 'Option 1', value: 'value1' },
        { label: 'Option 2', value: 'value2' },
        { label: 'Option 3', value: 'value3' }
      ],
      selectedValues: []
    };
  },
  methods: {
  }
};

</script>
