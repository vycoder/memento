<template>
  <section>
    <div class="order-now">
      <div class="heading">
        <p class="heading heading-4"> Availabe in e-book! Soon in Hardcopy!</p>
        <h2 class="heading-2">How to order</h2>
      </div>
      <p class="text">
        Order a softcopy for Php 200.00 via Bank of the Philippine Islands (BPI) <br>
        Account Number: 0589-2101-23 <br>
        Account Name: LOIDA CONCEPCION BAUTO
      </p>
      <p class="text">Send a picture of the receipt and wait for your copy on your facebook or email.</p>
      <p class="text">HARDCOPIES WILL BE AVAILABLE ON SEPTEMBER! Pre-order now!</p>
      <p class="text">Regular price is Php 249.00, order now and get a signed ADVANCE COPY for Php 199.00 only.</p>
      <button class="btn" @click="openURL('https://www.facebook.com/messages/t/loidaconcepcionbauto/')">Message Loida</button>
    </div>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'
.order-now {
  background-color rgba($primary, .05)
  display grid
  grid-gap 2rem
  padding 10rem
  align-content center
  justify-content center
  justify-items start
  min-height 100vh
  max-width 100%
  +respond-max($breakpoint-lg) {
    padding 0 5rem
  }
  +respond-max($breakpoint-md) {
    min-height 100%;
    padding 10rem
  }
  +respond-max($breakpoint-sm) {
    padding 8rem
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
