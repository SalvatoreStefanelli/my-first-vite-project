<script>
export default {
  name: 'App',
  data() {
    return {
      message: "Salvatore",
      background: "purple",
      movie: "",
    };
  },
  methods: {
    greetings() {
      console.log("ciao", this.message);
    },
  },
};
</script>

<template>
  <h1 :class="background">{{ message }}</h1>
  <button v-on:click="greetings">Click me</button>
  <label for="movie">Movie</label>
  <input id="movie" type="text" v-model="movie">
  <p>{{ movie }}</p>
</template>

<style></style>
