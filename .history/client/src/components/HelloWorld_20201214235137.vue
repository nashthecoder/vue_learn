<template>
  <div class="hello">
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
              Coming soon...
              </a>
            </p>
          </div>
        </li>
      </ul>
    </div>
    <hr />
    <div class="footer">
      NashTheCoder | Copyright © 2019-present MadHacks
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
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
</style>
