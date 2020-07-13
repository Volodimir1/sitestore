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
  <video autoplay loop>
    <source src="../videos/Earth-SS_7_2.mp4" type="video/mp4"/>
  </video>
  <!-- About -->
  <div class="header__center">
    <div class="header__center-item about">
      <h3 class="about__title">About us</h3>
      <p class="about__text">Do you think we will make you a website? Sorry, no.</p>
      <p class="about__text">We will fulfill your dream! This is just magic.</p>
    </div>
    <div class="header__center-item">
      <p></p>
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
  // background-image: url(../images/SSdimetria_2.JPG);
  // background-size: cover;
  // background-position: center center;
  // position: relative;
  // height: 100vh;
  // max-height: max-content;
  &__head {
      background-color: $N600;
      opacity: 0.9;
      position: relative;
      color: white;
      z-index: 1;
      @include flex(space-around, center);
      &:hover {
        opacity: 0.97;
      }
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
    border-radius: 17px;
    &:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 10px $T200;
    }
  }
  &__title-head {
    font-family: $title-font, cursive;
    @include text($H800, 400, $M1);
    text-align: center;
  }
  &__center {
    // width: 100%;
    // height: 100%;
    // height: 100vh;
    position: absolute;
    width: 100%;
    top: 25%;

    @include flex(space-between, center);
    padding: 50px;
  }
  &__center-item {
    // margin: auto;
    height: 400px;
    width: 400px;
    background-color: $N600;
    border-radius: 20px;
    opacity: 0.8;
  }
}
.header-item {
  &:not(:last-child) {
      margin-right: 40px;
    }
}
video {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  object-position: center;
  object-fit: cover;
}
.about {
  position: relative;
  color: $M1;
  z-index: 1;
  &__title {
    text-align: center;
  }
}
</style>