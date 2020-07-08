<template>
<div class="header">
    <div class="header-item header__title">
      <img class="header__title-item header__image" src="../images/sites2logo.svg" alt="logo">
      <h1 class="header__title-item header__title-head">Site Store</h1>
    </div>
    <div class="header-item header__nav">

    </div>
</div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String
  }
};
</script>

// <style scoped lang="scss">
.header {
  background-color: $N600;
  @include flex(space-around, center);
  &__title {
    @include flex(space-around, center);
  }
  &__title-item {
    &:not(:last-child) {
      margin-right: 10px;
    }
  }
  &__image {
    @include svg(35px, $N800)
    &:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 10px $T200;
    }
  }
  &__title-head {
    font-family: $title-font, cursive;
    @include text($H800, 400, $M1);
    text-align: center;
    // margin-top: 30px; 
  }
}
.header-item {
  &:not(:last-child) {
      margin-right: 40px;
    }
}
</style>