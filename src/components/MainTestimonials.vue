<template>
  <section class="main-testimonials">
    <div class="main-testimonials__head">
      <h2 class="main-testimonials__head-title">
        Testimonials
      </h2>
    </div>
    <div class="main-testimonials__body" v-for="testimonial in testimonials" :key="testimonial.id">
      <div class="main-testimonials__text">
        <div class="main-testimonials__text-star">
          <img src="/img/star.svg" alt="star" v-for="n in testimonial.stars">
        </div>
        <div class="main-testimonials__text-quote">
          {{ testimonial.text }}
        </div>
        <div class="main-testimonials__text-name">
          {{ testimonial.name }}
        </div>
        <div class="main-testimonials__text-position">
          {{ testimonial.position }}
        </div>
      </div>
      <div class="main-testimonials__image"> 
        <img class="main-testimonials__image-photo" :src="testimonial.image" alt="photo of the author of the review">
        <img src="/img/oval.svg" alt="Picture oval" class="main-testimonials__image-oval">
        <img src="/img/cross.svg" alt="Picture cross" class="main-testimonials__image-cross">
      </div>
      <div class="main-testimonials__buttons">
        <button>
          &lt;
        </button>
        <button>
          &gt;
        </button>
      </div>
    </div>
  </section>
</template>

<script>
import testimonials from '../data/testimonials'

export default ({
  name: 'MainTestimonials',
  data() {
    return {
      testimonials,
    }
  },
})
</script>

<style lang="scss">
  .main-testimonials {
    margin-top: 340px;
    position: relative;

    &__head {
      text-align: left;

      &-title {
        font-family: 'Playfair Display';
        font-weight: 700;
        font-size: 36px;
        line-height: 50px;
        color: #000000;
      }
    }

    &__body {
      display: flex;
      justify-content: space-between;
      text-align: left;

      &::before {
        position: absolute;
        content: '';
        width: 132px;
        height: 60px;
        background: #FFFFFF;
        border-radius: 16px 0px 0px 0px;
        bottom: 0;
        right: 0;
      }
    }

    &__text {
      width: 450px;
      color: #000000;

      &-star {
        margin-top: 145px;
        
        img {
          margin-right: 18px;
        }
      }

      &-quote {
        margin-top: 30px;
        font-family: 'Mulish';
        font-weight: 400;
        font-size: 24px;
        line-height: 36px;
      }

      &-name {
        margin-top: 40px;
        font-family: 'Inter';
        font-weight: 700;
        font-size: 22px;
      }

      &-position {
        font-family: 'Inter';
        font-weight: 400;
        font-size: 18px;
        line-height: 48px;
        color: rgba(0, 0, 0, 0.85);
      }
    }

    &__image {
      margin-top: 60px;
      width: 385px;
      height: 490px;
      overflow: hidden;
      border-radius: 14px;

      &-photo {
        height: 490px;
      }

      &-oval {
        position: absolute;
        top: 120px;
        right: -15px;
        width: 42px;
        z-index: -1;
      }

      &-cross {
        position: absolute;
        width: 32px;
        bottom: -13px;
        right: 365px;
        transform: rotate(8.17deg);
      }
    }

    &__buttons {
      position: absolute;
      bottom: 0;
      right: 0;
    }
  }
</style>
