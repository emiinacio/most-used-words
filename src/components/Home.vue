<template>
  <v-container fluid>
      <div class="pills">
        <Pill v-for="word in groupedWord" :key="word.name" 
        :name="word.name" :amount="word.amount"/>
      </div>
  </v-container>
</template>

<script>
import Pill from "./Pill.vue";

export default {
  name: "App",
  components: { Pill },
  data: function () {
    return {
      groupedWord: [
        { name: "i", amount: 1234 },
        { name: "you", amount: 900 },
        { name: "he", amount: 853 },
      ],
    };
  },
};
</script>

<style>
    .pills {
        display: flex;
    }
</style>
