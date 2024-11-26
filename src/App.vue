<template>
  <div id="app">
    <header>
      <h1>Chuck Norris Jokes</h1>
    </header>
    <ul>
      <li v-for="(joke, index) in jokes" :key="index">
        {{ joke.value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      jokes: [
        { value: "Chuck Norris can skydive into outer space." },
        { value: "The chief export of Chuck Norris is pain." },
        { value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { value: "Time waits for no man. Unless that man is Chuck Norris." },
        { value: "If you spell Chuck Norris in Scrabble, you win. Forever." },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Arial, sans-serif;
  text-align: center;
  color: #333;
  background: #f4f4f9;
  padding: 20px;
}
header {
  background-color: #222;
  color: #fff;
  padding: 10px 0;
}
h1 {
  margin: 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  margin: 10px 0;
  padding: 10px;
  border: 1px solid #ccc;
  background: #fff;
  border-radius: 5px;
}
</style>
