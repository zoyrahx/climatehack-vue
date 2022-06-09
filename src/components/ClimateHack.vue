
<template>
  <div class="climateHack">
    <h1>{{ msg }}</h1>
    <h4>AVERA</h4>

    <p>Automated Vessel Emission and Route Analysis</p>
    <iframe width="560" height="315" src="https://app.powerbi.com/groups/me/reports/add09b10-90d7-47ac-879a-d3e3f551bff5/ReportSection"></iframe>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  name: 'ClimateHack',
  props: {
    msg: String
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
