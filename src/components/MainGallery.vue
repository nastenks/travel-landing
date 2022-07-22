<template>
  <section class="main-gallery">
    <div class="main-gallery__head">
      <h2 class="main-gallery__head-title">
        Featured destinations
      </h2>
      <a href="/gallery" class="main-gallery__head-link">
        View all >
      </a>
    </div>
  </section>
</template>

<script>
import item-gallery from '../assets/item-gallery.js';

export default ({
  name: 'MainGallery',
})
</script>

<style lang="scss">
  .main-gallery {
    margin-top: 400px;

    &__head {
      display: flex;
      justify-content: space-between;
      align-items: center;

      &-title {
        font-family: 'Playfair Display', sans-serif;
        font-weight: 700;
        font-size: 36px;
        line-height: 50px;
        color: #000000;
      }

      &-link {
        font-family: 'Inter', sans-serif;
        font-weight: 600;
        font-size: 17px;
        color: #FB8F1D;
      }
    }
  }
</style>