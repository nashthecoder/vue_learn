<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h3>Learning Chart.js</h3>
    <hr />
    <div class="features">
      <ul>
        <li>
          <div class="feature">
            <h2>Header</h2>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </div>
        </li>
        <li>
          <div class="feature">
            <h2>Header</h2>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
            </p>
          </div>
        </li>
        <li>
          <div class="feature">
            <h2>Header</h2>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua.
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
