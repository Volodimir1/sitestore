<template>
<div class="header">
  <!-- header up -->
  <div class="header__head">
    <div class="header-item header__title">
      <!-- <img class="header__title-item header__image" src="../images/sites2logo.svg" alt="logo"> -->
      <img class="header__title-item header__image" src="../images/SSdimetria_2_3_logo.png" alt="logo">
      <h1 class="header__title-item header__title-head">Site Store</h1>
    </div>
    <div class="header-item header__nav">
      <label class="burger navigation__burger">
        <input class='burger__input' type="checkbox">
        <span class="burger__box">
          <span class="burger__item"></span>
          <span class="burger__item"></span>
          <span class="burger__item"></span>
        </span>
        <!-- Hack -->
        <span class="navigation__list burger__menu">
          <span class="navigation__item">
            <a class="navigation__link" href="#home">Home</a>
          </span>
          <span class="navigation__item">
            <a class="navigation__link" href="#about">About</a>
          </span>
          <span class="navigation__item">
            <a class="navigation__link" href="#gallery">Catalog</a>
          </span>
          <span class="navigation__item">
            <a class="navigation__link" href="">Contact</a>
          </span>
        </span>
      </label>
    </div>
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
  background-image: url(../images/SSdimetria_2_1_background.png);
  background-size: cover;
  background-position: center center;
  position: relative;
  height: 100vh;
  max-height: max-content;
  &__head {
      background-color: $N600;

      @include flex(space-around, center);
  }
  &__title {
    @include flex(space-around, center);
  }
  &__title-item {
    &:not(:last-child) {
      margin-right: 10px;
    }
  }
  &__image {
    // @include svg(35px, $N800)
    height: 35px;
    width: 35px;
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