<script>
import axios from "axios";
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
  name: "AppVue",
  components: {
    AppHeader,
    AppMain,
  },
  data() {
    return {
      characters: [],
      archetype: [],
    };
  },
  created() {
    axios
      .get("https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0")
      .then((response) => {
        this.characters = response.data.data.slice(0, 20);
      });
  },
};
</script>

<template>
  <AppHeader></AppHeader>
  <AppMain
    :charactersList="characters"
    :charactersCount="characters.length"
    :archetypes="archetype"
  ></AppMain>
</template>

<style lang="scss"></style>
