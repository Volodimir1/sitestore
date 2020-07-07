<template>
<div class="header">
    <img class="header__image" src="../images/sites2logo.svg" alt="logo">
    <h1 class="header__title">Site Store</h1>
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
    // margin: 0;
    &__image {
      height: 30px;
      width: 30px;
    }
    &__title {
      font-family: $title-font, cursive;
      @include text($H800, 400, $M1);
      text-align: center;
      // margin-top: 30px; 
    }
}
</style>