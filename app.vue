<template>
  <div>
    <div class="container">
      <h1>Old Faithful Geyser Data</h1>
      <!-- Bootstrap grid system -->
      <div class="row align-items-start">
        <div class="col-4">
          <label for="customRange1" class="form-label">Number of bins:</label>
          <input type="range" class="form-range" id="customRange1" min=1 max=30 value=10 @input="updateSelected">
          <div id="bins">Selected: {{ selectedValue }}</div>
        </div>
        <div class="col-8">
          <div>
            <!-- Where we'll get the chart drawn -->
            <canvas id="myChart"></canvas>
          </div>
        </div>
      </div>
    </div>
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