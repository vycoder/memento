<template>
  <section>
    <ul>
      <li>Learn more about AVM</li>
      <li>AVM Phillipines</li>
      <li>Read more about her story</li>
    </ul>
    <p class="text-center text-white q-pt-xl q-pb-md">
      &copy; Copyright 2018 by <span class="webmaster" @click="openURL('www.josephharveyangeles.com')">Joseph Harvey C. Angeles</span>, a friend. While having an AVM is a bit of a bummer, I'm not worried that she won't eventually recover, at the very least, she'll probably just use it to make her life more meaningful &mdash; that's just how she rolls.
    </p>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'
ul {
  list-style none
  padding 0 8rem
  display grid
  grid-template-columns repeat(auto-fit, minmax(15rem, 1fr))
  grid-gap 2rem
  justify-content center
  align-items center
  flex-wrap wrap

  li {
    color white
    display block
    font-family $font-primary
    font-size 1.5rem
    cursor pointer
    padding 2rem
    text-align center
    transition all .2s ease
    &:hover {
      background-color rgba($primary, .5)
    }
  }
}
p {
  width 60%
  margin 0 auto
}
.webmaster {
  cursor pointer
  transition all .3s ease
  display inline-block
  &:hover {
    transform rotate(-10deg) scale(1.5)
    color pink
    background-color rgba($secondary, .8)
    box-shadow 0rem 2rem 2rem rgba(#000, .2)
  }
}
</style>
<script>
import {openURL} from 'quasar'
export default {
  methods: {
    openURL
  }
}
</script>
