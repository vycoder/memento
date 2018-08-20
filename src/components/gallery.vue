<template>
  <section>
    <figure class="gallery__item--1">
      <img src="~assets/gallery/1.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--2">
      <img src="~assets/gallery/2.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--3">
      <img src="~assets/gallery/4.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--4">
      <img src="~assets/gallery/3.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--5">
      <img src="~assets/gallery/5.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--6">
      <img src="~assets/gallery/6.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--7">
      <img src="~assets/gallery/7.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--8">
      <img src="~assets/gallery/8.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--9">
      <img src="~assets/gallery/9.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--10">
      <img src="~assets/gallery/10.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--11">
      <img src="~assets/gallery/11.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--12">
      <img src="~assets/gallery/12.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--13">
      <img src="~assets/gallery/13.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--14">
      <img src="~assets/gallery/14.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--15">
      <img src="~assets/gallery/15.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--16">
      <img src="~assets/gallery/16.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--17">
      <img src="~assets/gallery/17.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--18">
      <img src="~assets/gallery/18.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--19">
      <img src="~assets/gallery/20.jpg" class="gallery__img">
    </figure>
    <figure class="gallery__item--20">
      <img src="~assets/gallery/19.jpg" class="gallery__img">
    </figure>
  </section>
</template>
<style lang="stylus" scoped>
@import '~variables'

section {
  display grid
  grid-template-columns repeat(11, 1fr)
  grid-template-rows repeat(8, 5vw)
  grid-gap 1.5rem
  padding 1.5rem
  background-color rgba($primary, 0.05)
  & > figure {
    transition all .2s ease
    cursor pointer
    &:active {
      transform scale(1.3)
      box-shadow 0 0 20rem rgba(#000, .9)
    }
  }
}
.gallery__item {
  &--1 {
    grid-row 1 / span 3
    grid-column 1 / span 2
  }

  &--2 {
    grid-row 1 / span 2
  }

  &--3 {
    grid-row 1 / span 2
    grid-column 4 / span 2
  }

  &--4 {
    grid-row 1 / 2
    grid-column 6 / span 2
  }

  &--5 {
    grid-row 1 / span 3
    grid-column 8 / span 2
  }

  &--6 {
    grid-row 1 / span 2
    grid-column 10 / -1
  }

  &--7 {
    grid-row 4 / span 2
    grid-column 1 / span 2
  }

  &--8 {
    grid-row 3 / span 3
    grid-column span 2
  }

  &--9 {
    grid-row 3 / span 2
  }

  &--10 {
    grid-row 2 / span 4
    grid-column 6 / span 2
  }

  &--11 {
    grid-row 3 / span 3
    grid-column 10 / span 2
  }

  &--12 {
    grid-row 4 / span 2
    grid-column 8 / span 2
  }

  &--13 {
    grid-row 5 / span 2
    grid-column 5
  }

  &--14 {
    grid-row 6 / span 3
    grid-column 9 / span 3
  }

  &--17 {
    grid-row 7 / span 2
    grid-column 1 / span 2
  }

  &--18 {
    grid-row 6 / -1
    grid-column 3 / span 2
  }

  &--19 {
    grid-row 7 / -1
  }

  &--20 {
    grid-row 6 / -1
    grid-column 6 / span 3
  }
}
.gallery__img {
  width 100%
  height 100%
  object-fit cover
  display block
}
</style>
