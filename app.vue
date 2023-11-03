<template>
  <div>
    <div class="notifictation-header"
      style="padding: 25px;background-color: rgb(206, 122, 122);margin-bottom: 30px;color:white;font-weight: 700;">
      <div class="notification-header-title">
        <span>This is the feature working branch</span>
      </div>
    </div>
    <div class="container">
      <h1>Old Faithful Geyser Data</h1>
      <!-- Bootstrap grid system -->
      <div class="row align-items-start">
        <LeftPanel />
        <div class="col-8">
          <div>
            <CreateChart />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>