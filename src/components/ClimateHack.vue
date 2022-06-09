
<template>
  <div class="climateHack">
    <h1>{{ msg }}</h1>
    <h4>AVERA</h4>

    <p>Automated Vessel Emission and Route Analysis</p>
    <iframe title="AVERA Dashboard" width="1140" height="541.25" src="https://app.powerbi.com/reportEmbed?reportId=add09b10-90d7-47ac-879a-d3e3f551bff5&autoAuth=true&ctid=e93c0c9e-286e-4c79-b4cd-be2a9d8ccf16&config=eyJjbHVzdGVyVXJsIjoiaHR0cHM6Ly93YWJpLXNvdXRoLWVhc3QtYXNpYS1yZWRpcmVjdC5hbmFseXNpcy53aW5kb3dzLm5ldC8ifQ%3D%3D" frameborder="0" allowFullScreen="true"></iframe>
  </div>
</template>

<script>


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
