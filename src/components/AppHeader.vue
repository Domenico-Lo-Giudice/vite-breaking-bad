<script>
export default {
  data() {
    return {
      title: "Header",
    };
  },
};
</script>

<template>
  <header class="header-bg">
    <div class="container">
      <div class="row d-flex align-items-center">
        <div class="col-2">
          <img
            class=""
            src=".././assets/TCG_logo_500x500.png"
            alt=""
          />
        </div>
        <div class="col">
          <h1>Yu-Gi-Oh Api</h1>
        </div>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header-bg {
  background-color: white;
}
img {
  height: 150px;
}
</style>
