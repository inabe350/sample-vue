<template>
  <header class="header">
    <header-nav />
  </header>
</template>

<style lang="scss" scoped>
.header {
  padding: 16px 40px;
  background-color: rgba($color: $colorWhite, $alpha: 0.8);
  @media #{$sp} {
    padding: 8px 4.3%;
  }
}
</style>
