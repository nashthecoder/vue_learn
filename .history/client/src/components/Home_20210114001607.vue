<template>
  <div class="hello">
    <button class="btn">Bar</button>
    <button class="btn">Bubble</button>
    <button class="btn">Donut</button>
    <button class="btn">Line</button>
    <button class="btn">Pie</button>
    <button class="btn">Polar</button>
    <button class="btn">Radar</button>
    <button class="btn">Scatter</button>
     <v-btn
      rounded
      @click="BarChart"
    >
      Bar
    </v-btn>

    <h1>{{ msg }}</h1>
    <hr />
    <div class="features">
      <ul>
        <li>
          <div class="feature">
            <h2>Beginner</h2>
            <p>
              Resources: <br />
              <a href="https://canvasjs.com/"> Canvasjs.com</a> <br />
              <a href="https://www.chartjs.org/"> Chartjs.org</a>
              <br />
            </p>
          </div>
        </li>
        <li>
          <div class="feature">
            <h2>Intermediate</h2>
            <p>
              Resources: <br />
              <a href="https://learning.oreilly.com/library/view/learn-chartjs">
                Learn Chart.js
              </a>
              <br />
              <br />
            </p>
          </div>
        </li>
        <li>
          <div class="feature">
            <h2>Advanced</h2>
            <p>
              Resources: <br />
              <a href="https://d3js.org/">
                Coming soon..
              </a>
              <br />
              <br />
            </p>
          </div>
        </li>
      </ul>
    </div>
    <hr />
    <div class="footer">
      NashTheCoder | Copyright © 2020
    </div>
  </div>
</template>

<script>
import BarChart from "./BarChart.vue";
export default {
  name: "Home",
  BarChart,
  props: {
    msg: String
  }
};
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
.feature {
  padding: 1.2 rem 0;
  margin-top: 2.5 rem;
}
.btn {
  margin-left: 5px;
  margin-right: 5px;
  border-color: #42b983;
  width: 8%;
  font-weight: 600;
}
</style>
