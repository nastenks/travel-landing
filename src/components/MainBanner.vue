<template>
  <div class="banner">
    <div class="banner__text">
      <h1 class="banner__title">Explore and <br> Travel</h1>
      <p class="banner__descr">Holiday finder</p>
    </div>
    <div class="banner__image">
      <img src="/img/banner_image.png" alt="Picture on the banner">
    </div>
  </div>
</template>

<script>
export default ({
  name: 'MainBanner',
});
</script>

<style lang="scss">
  .banner {
    position: relative;
    display: flex;
    justify-content: space-between;
    margin-top: 80px;

    &__text {
      color: #202336;
      text-align: left;

      h1 {
        margin-bottom: 74px;
        font-family: 'Playfair Display', sans-serif;
        font-weight: 700;
        font-size: 64px;
      }

      &__descr {
        font-family: 'Inter';
        font-weight: 600;
        font-size: 22px;
      }

      p {
        &:before {
          display: block;
          position: absolute;
          height: 2px;
          width: 32px;
          background: #202336;
          bottom: -1px;
          content: "";
          left: 0;
        }
      }
    }

    &__image {
      img {
        position: absolute;
        right: -100px;
        width: 687px;
        height: 654px;
      }
    }
  }
</style>
