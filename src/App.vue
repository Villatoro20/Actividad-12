<template>
  <div id="app">
    <header>
      <h1>Chuck Norris Jokes</h1>
    </header>
    <div class="container">
      <div class="row">
        <chuck-card
          v-for="(joke, index) in jokes"
          :key="index"
          :icon-url="joke.icon_url"
          :value="joke.value"
        />
      </div>
    </div>
  </div>
</template>

<script>
import ChuckCard from './components/ChuckCard.vue';

export default {
  components: {
    ChuckCard,
  },
  data() {
    return {
      jokes: [
        {
          icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
          value: "Chuck Norris can skydive into outer space.",
        },
        {
          icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
          value: "The chief export of Chuck Norris is pain.",
        },
        {
          icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
          value: "Chuck Norris doesn't read books. He stares them down until he gets the information he wants.",
        },
        {
          icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
          value: "Time waits for no man. Unless that man is Chuck Norris.",
        },
        {
          icon_url: "https://assets.chucknorris.host/img/avatar/chuck-norris.png",
          value: "If you spell Chuck Norris in Scrabble, you win. Forever.",
        },
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
</style>

