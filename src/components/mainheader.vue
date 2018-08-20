<template>
  <section>
    <figure>
      <img src="~assets/logo.png" alt="memento logo" class="logo-img" />
      <figcaption>
        <h4 class="heading heading-4">Memento</h4>
      </figcaption>
    </figure>
    <h4 class="heading heading-5">An AVM Survivor Story</h4>
    <h1 class="heading heading-1">Galaw-galaw baka ma-stroke</h1>
    <button class="btn" @click="scroll('#scrollSnap')">Order now</button>
    <div class="seenon">Seen on</div>
    <div class="seenon-logos">
      <img src="~assets/gma-logo.png" alt="GMA 7">
      <img src="~assets/mpklm.png" alt="Magpakailanman">
      <img src="~assets/abscbn-logo.png" alt="ABS-CBN">
      <img src="~assets/UMKlogo.png" alt="Umagang kay ganda">
    </div>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'
section {
  padding 6rem
  padding-top 4rem
  display grid
  grid-row-gap 1.5rem
  grid-template-rows 1fr min-content minmax(6rem, min-content) 1fr
  grid-template-columns minmax(min-content, auto)
  background-image linear-gradient(rgba($secondary, .9), rgba($secondary, .9)), url('~assets/bg2.jpg')
  background-size cover
  background-position center
  height 100%
  justify-content center
}

.heading-4 {
  text-transform uppercase
  letter-spacing 1rem
  margin-left 1rem
}

.btn {
  align-self start
  justify-self start
}

figure {
  display flex
  align-items center
  justify-content center
}

.logo-img {
  height 3rem
}

.seenon {
  display grid
  grid-template-columns 1fr max-content 1fr
  font-size 1.6rem
  font-family $font-primary
  text-transform uppercase
  color white
  align-items center
  grid-column-gap 1.5rem
  &::before,
  &::after {
    content ""
    display block
    height 1px
    background-color currentColor
  }
}

.seenon-logos {
  display grid
  grid-template-columns repeat(4, 1fr)
  grid-gap 3rem
  justify-items center
  align-items center
  justify-content center
  img {
    max-height 4rem
    max-width 100%
    filter: brightness(70%)
  }
}
</style>
<script>
import scroller from 'vue-scrollto/src/scrollTo'
export default {
  methods: {
    scroll (elementId, duration = 1000, delay = 100) {
      setTimeout(() => {
        scroller(elementId, duration)
      }, delay)
    }
  }
}
</script>
