<template>
  <ol>
    <li v-for="item in tasks" :key="item">
      {{ item }}
    </li>
  </ol>
</template>

<script>
export default {
  name: "Agenda",
  props: {
    tasks: Array,
  },
};
</script>

<style scoped>
ol {
  text-align: left;
  width: 500px;
  margin: 0 auto;
}
</style>
