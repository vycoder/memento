<template>
  <section>
    <h4 class="heading heading-5">Links</h4>
    <div class="links-list">
      <img src="~assets/loida.jpg" alt="Loida Bauto" class="links-list__img">
      <div class="links-list__item" @click="openURL('https://www.facebook.com/loidaconcepcionbauto')">
        <h5 class="heading heading-4--light">Loida Bauto</h5>
        <p class="subtitle">Author</p>
      </div>
      <img src="~assets/mementogroup.jpg" alt="Memento" class="links-list__img">
      <div class="links-list__item" @click="openURL('https://www.facebook.com/MementoNiLoida/?hc_ref=ARSKnh8Z4BKPQibqhifJAcys5PG6Ia-1kydb3JT2LBdKokAcmDxC7cOx6l_VRpjY5-8&fref=nf&__tn__=kC-R')">
        <h5 class="heading heading-4--light">@MementoNiLoida</h5>
        <p class="subtitle">Facebook page</p>
      </div>
      <img src="~assets/avmgroup.jpg" alt="AVM Group" class="links-list__img">
      <div class="links-list__item" @click="openURL('https://www.facebook.com/AVMPhilippines/?hc_ref=ARRWVO7ZA55oLPJYXKSkWJ_eAQ2WQyTbFNjoHPGj0VkTm_k9El_Jfyen-dHQRrUxZkA&fref=nf&__tn__=kCH-R')">
        <h5 class="heading heading-4--light">@AVMPhilippines</h5>
        <p class="subtitle">AVM Community</p>
      </div>
    </div>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'
section {
  display flex
  flex-direction column
  justify-content center
  align-items center
  height 100%
  padding 3rem 0

}

h5 {
  color rgba(white, 0.7)
  transition all .3s ease
}

.links-list {
  display grid
  grid-template-columns min-content max-content
  +respond-max($breakpoint-lg) {
    grid-template-columns repeat(3, min-content max-content)
  }
  +respond-max($breakpoint-sm) {
    grid-template-columns min-content max-content
  }
  grid-column-gap 2rem
  grid-row-gap 5vh
  align-items center
  &__item {
    cursor pointer
    &:hover h5 {
      color white
    }
  }
  &__img {
    width 7rem
    border-radius 50%
    display block
  }
}

.subtitle {
  font-family $font-primary
  color white
  font-size 1.3rem
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
