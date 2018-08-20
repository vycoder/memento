<template>
  <q-page>
    <div class="container">
      <header class="header">
        <heading />
      </header>
      <div class="sideheader">
        <sideheading />
      </div>
      <div class="testimonials q-py-xl">
        <testimonials />
      </div>
      <div class="books">
        <books />
      </div>
      <div id="scrollSnap" class="order-now">
        <order-now />
      </div>
      <div class="video q-py-xl">
        <q-video src="https://www.youtube.com/embed/sV38f_5Tcvc" />
      </div>
      <div class="story q-py-xl">
        <story/>
      </div>
      <div class="gallery">
        <gallery />
      </div>
      <footer class="footer q-py-md">
        <feeter />
      </footer>

    </div>
  </q-page>
</template>

<style lang="stylus" scoped>
@import '~variables'
.container {
  display grid
  grid-template-rows 80vh min-content 100vh repeat(3, min-content)
  grid-template-columns \[full-start\] minmax(6rem, 1fr) \[center-start\] repeat(8, \[col-start\] minmax(min-content, 14rem) \[col-end\]) \[center-end\] minmax(6rem, 1fr) \[full-end\]
  +respond-max($breakpoint-lg) {
    grid-template-rows 80vh repeat(2, min-content) 100vh repeat(3, min-content)
  }
}

.header {
  grid-column full-start / col-end 6
  +respond-max($breakpoint-lg) {
    grid-column full-start / full-end
  }
}

.sideheader {
  background-color $secondary
  grid-column col-start 7 / full-end
  +respond-max($breakpoint-lg) {
    grid-column full-start / full-end
  }
}

.testimonials {
  grid-column center-start / center-end
}

.books {
  grid-column full-start / col-end 4
  +respond-max($breakpoint-md) {
    grid-column full-start / full-end
  }
}

.order-now {
  grid-column col-start 5 / full-end
  +respond-max($breakpoint-md) {
    grid-column full-start / full-end
  }
}

.video {
  grid-column full-start / full-end
  background-image linear-gradient(rgba($primary, 0.05), rgba($primary, 0.1), white)
  /deep/ .q-video {
    margin 0 auto
    height 30vw
    width 30vw
  }
}

.story {
  grid-column full-start / full-end
  width 70%
  margin 0 auto
}

.gallery {
  grid-column full-start / full-end
}

.footer {
  grid-column full-start / full-end
  background-color $secondary
  padding-top 7rem
}
</style>

<script>
import Heading from 'components/mainheader'
import Sideheading from 'components/sideheader'
import Story from 'components/story'
import Books from 'components/books'
import OrderNow from 'components/order-now'
import Testimonials from 'components/testimonials'
import Gallery from 'components/gallery'
import Feeter from 'components/footer'
export default {
  name: 'PageIndex',
  components: { OrderNow, Story, Gallery, Books, Feeter, Heading, Sideheading, Testimonials }
}
</script>
