<template>
<div class="header">
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
    &__title {
       font-family: $title-font, cursive;
       @include text($H800, 400, $M1);
      text-align: center;
        margin-top: 30px; 
    }
}
</style>