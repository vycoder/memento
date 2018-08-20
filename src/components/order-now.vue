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
      <p class="text">
        OR via Smart PADALA<br>
        5299-6761-3152-8107<br>
        Send to: 09081557234
      </p>
      <p class="text">Send a picture of the receipt and wait for your copy on your facebook or email.</p>
      <p class="text">HARDCOPIES WILL BE AVAILABLE SOON! Pre-order now!</p>
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
  align-content center
  justify-items start
  padding 10rem
  height 100vh
  max-width 100%
  +respond-max($breakpoint-sm) {
    padding 5rem;
    height 100%
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
