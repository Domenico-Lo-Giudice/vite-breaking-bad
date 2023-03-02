<script>
import AppCard from "./AppCard.vue";
export default {
  name: "AppMain",
  components: {
    AppCard,
  },
  props: {
    charactersList: {
      type: Array,
    },
    charactersCount: {
      type: Number,
    },
    archetypes: {
      type: Array,
    },
  },
};
</script>

<template>
  <div class="deckCont">
    <div class="container">
      <div class="row">
        <div class="col mt-5">
          <select
            name=""
            id=""
          >
            <option value="">Alien</option>
          </select>
        </div>
      </div>
    </div>

    <div class="container bg-light mt-3 rounded">
      <div class="row bg-dark rounded-top py-3">
        <h3 class="text-light">
          Sono state trovate {{ charactersCount }} carte
        </h3>
      </div>

      <div class="row">
        <div
          class="col-2"
          v-for="character in charactersList"
        >
          <AppCard :character="character"></AppCard>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.deckCont {
  background-color: goldenrod;
  height: 2100px;
}
</style>
