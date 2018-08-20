<template>
  <section>
    <div class="books__cover">
      <img src="~assets/hardcopy.png" alt="hardcopy" class="books__cover--img-1">
      <img src="~assets/softcopy.jpg" alt="softcopy" class="books__cover--img-2">
    </div>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'
.books__cover {
  background-image linear-gradient(rgba($secondary, .5), rgba($secondary, .5)), url('~assets/order-now-bg.jpg')
  background-size cover
  position relative
  display block
  height 100vh

  &--img-1 {
    box-shadow 0 3rem 5rem rgba(#fff, .1)
    position absolute
    width 45%
    top 50%
    left 35%
    transform translate(-50%, -50%)
    z-index 1
    max-width 100%
  }

  &--img-2 {
    box-shadow 0 3rem 5rem rgba(#000, .7)
    width 35%
    position absolute
    top 55%
    left 65%
    z-index 2
    transform translate(-50%, -50%) rotate(15deg)
    max-width 100%
  }
}
</style>
