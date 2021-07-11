<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Agenda :tasks="agenda" />
</template>

<script>
import Agenda from "./components/Agenda.vue";

export default {
  name: "App",
  data() {
    return {
      agenda: [
        "Підготовка середовища розробки",
        "Створення нового проекту за допомогою vue-cli",
        "Базовий Vue",
        "Розгортання проекту на Netlify",
        "Наступні кроки.",
      ],
    };
  },
  components: {
    Agenda,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
