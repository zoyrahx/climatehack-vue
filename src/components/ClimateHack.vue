
<template>
  <div class="climateHack">
    <h1>{{ msg }}</h1>
    <h4>Team Epsilon</h4>

    <p>Sample page</p>
    <iframe width="560" height="315" src="https://public.tableau.com/views/MeasuringReactionsReactionAnalytics/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link&:embed=yes&:tabs=yes&:toolbar=yes"></iframe>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  name: 'ClimateHack',
  props: {
    msg: String
  },
  data() {
    return {
      data: [],
    };
  },
  mounted(){
    this.getData();
  },
  methods: {
    async getData() {
      try {
        const response = await axios.get(
          "http://localhost:8000/"
        );
        this.data = response.data;
      } catch (error) {
        console.log(error);
      }
    },
  },
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
