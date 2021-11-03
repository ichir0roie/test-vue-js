<template>
  <h1>{{ msg }}</h1>
  <!-- <div id="counter">{{ counter }}</div> -->
  <div id="counter">{{ counterT }}</div>
  <!-- <div id="counter">{{ testValue }}</div> -->
</template>

<script>
export default {
  name: "Counter",
};

import { createApp } from "vue";

const Counter = {
  data: {
    counterT: 0,
  },
  mounted() {
    setInterval(() => {
      this.counterT++;
      console.log(this.counterT);
    }, 1000);
  },
};

createApp(Counter).mount("#counter");
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
div {
  color: white;
  background: black;
  width: max-content;
  height: max-content;
  font-size: 50px;
}

h1 {
  color: gray;
  background: darkgrey;
}
</style>
