<template>
  <div>
      <span>{{name}}</span>
      <span>{{amount}}</span>
  </div>
</template>

<script>

export default {
  name: "App",
  props: ["name", "amount"],
};
</script>

<style>
</style>