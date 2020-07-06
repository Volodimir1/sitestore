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
       font-family: 'Modak', cursive;
    //    @include text($H700, 400, $M1);
            //   color: $M1;

    //    font-size: 3em;
    //    font-weight: normal;
        // -webkit-font-smoothing: antialiased;
        // -moz-osx-font-smoothing: grayscale;
        text-align: center;
        // color: #FDB100;
        margin-top: 30px; 
    }
}
</style>