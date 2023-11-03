<template>
  <div class="col-4">
    <label for="customRange1" class="form-label">Number of bins:</label>
    <input type="range" class="form-range" id="customRange1" min=1 max=30 value=10 @input="updateSelected">
    <div id="bins">Selected: {{ selectedValue }}</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selectedValue: 22, // Initial value
    };
  },
  methods: {
    updateSelected(event) {
      this.selectedValue = event.target.value;
    },
  },
};
</script>