<template>
  <div class="home-view">
    <img class="bg-img" src="@/assets/imgs/main.jpg" alt="" />
  </div>
</template>

<style lang="scss" scoped>
.home-view {
  padding-top: 7svh;
  min-height: 100svh;

  > .bg-img {
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
