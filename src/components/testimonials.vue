<template>
  <section>
    <div class="testimonial">
      <h4 class="heading heading-4">Life Changing</h4>
      <p class="text">I cried a lot, laughed a lot, learned a lot, and loved every single detail and lesson of the story. You never treat your situation as an excuse to take your life away but rather change others' lives radically. And I'm one of those.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">#Blessed</h4>
      <p class="text">Random ko lang 'to nakita. Tapos na-curious ako sa title. 'Di ko akalain na magiging blessing to sakin.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Truly heart touching</h4>
      <p class="text">A truly heart touching story, brilliantly written sprinkled with sense of humor and bits of life morals.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Heart and Humor</h4>
      <p class="text">What a wonderful look into the ups and downs of life... An autobiography rich with heart and humor.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Roller coaster storytelling</h4>
      <p class="text">It's an eye opener. It's a roller coaster storytelling punctuated with laughs, sighs and realizations. Good job.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Inspirational</h4>
      <p class="text">It was very inspirational at punong puno ng puso! Grabe, medyo roller coaster and emotion kapag binasa.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Eye-opening</h4>
      <p class="text">Ang galing... Wala akong maicomment eh. Reading your story is really a big eye opener.</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Pak!</h4>
      <p class="text">...truly, heart breaking however courageously well written. Tagalog na tagalog. Pak!</p>
    </div>
    <div class="testimonial">
      <h4 class="heading heading-4">Heart-racing</h4>
      <p class="text">Bumibilis tibok ng puso ko habang binabasa ko ito.</p>
    </div>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'
section {
  display grid
  grid-template-columns repeat(auto-fit, minmax(25rem, 1fr))
  grid-gap 5rem
}
.heading {
  letter-spacing .3rem
}
.testimonial {
  position relative
  z-index 0
  &::before {
    content "\201C"
    position absolute
    top -4.5rem
    left -4.5rem
    color rgba($primary, .06)
    font-family sans-serif
    font-size 20rem
    line-height 1
  }
}
</style>
