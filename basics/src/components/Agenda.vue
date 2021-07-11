<template>
  <ol>
    <li v-for="(item, index) in tasks" :key="index">
      {{ item }}
    </li>
  </ol>
</template>

<script>
export default {
  name: "Agenda",
  props: { tasks: Array },
};
</script>

<style scoped>
ol {
  text-align: left;
}
</style>
