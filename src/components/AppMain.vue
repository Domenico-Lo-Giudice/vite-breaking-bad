<script>
export default {
  data() {
    return {
      title: "Main",
    };
  },
};
</script>

<template>
  <div class="Main">
    <div class="container">
      <div class="row">
        <div class="mt-3">
          <select
            name=""
            id=""
          >
            <option selected>Alien</option>
          </select>
        </div>
      </div>
    </div>
    <div class="main-cards-container container bg-light mt-5">CARDS</div>
  </div>
</template>

<style lang="scss" scoped>
.Main {
  background-color: orange;
  height: 3000px;
}

.main-cards-container {
  height: 1500px;
}
</style>
