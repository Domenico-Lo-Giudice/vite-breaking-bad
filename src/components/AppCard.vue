<script>
export default {
  name: "AppCard",
  props: {
    character: Object,
    archetype: Object,
  },
};
</script>

<template>
  <div class="card text-center my-1">
    <img
      :src="character.card_images[0].image_url"
      :alt="character.name"
    />
    <div class="card-body">
      <h5 class="card-title text-light">{{ character.name }}</h5>
      <p class="card-text fw-bolder">{{ character.archetype }}</p>
      <div>{{ character.type }}</div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  background-color: goldenrod;
}
</style>
