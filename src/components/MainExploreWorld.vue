<template>
  <section class="explore-world">
    <div class="explore-world__image">
      <img src="/img/banner_image.png" alt="Picture on the banner" class="explore-world__image-man">
    </div>
    <div class="explore-world__text">   
      <h2 class="explore-world__title">A new way to explore the world</h2>
      <p class="explore-world__descr">For decades travellers have reached for Lonely Planet books when looking to plan and execute their perfect trip, but now, they can also let Lonely Planet Experiences lead the way</p>
      <button class="explore-world__button base-button base-button_orange">Learn more</button>
    </div>
  </section>
</template>

<script>
export default ({
  name: 'MainExploreWorld',
});
</script>

<style lang="scss">
  .explore-world {
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
        position: relative;

        &:before {
          display: block;
          position: absolute;
          height: 2px;
          width: 32px;
          background: #202336;
          bottom: -18px;
          content: "";
          left: 0;
        }
      }
    }

    &__image {
      position: relative;

      &-man {
        position: absolute;
        right: -100px;
        width: 687px;
        height: 654px;
      }

      &-cross {
        position: absolute;
        right: 670px;
        top: 60px;
      }

      &-oval {
        &_bottom {  
          position: absolute;
          right: 600px;
          bottom: -100px;
        }

        &_left {
          position: absolute;
          right: 1200px;
          top: 310px;
        }
      }
    }

    &__form {
      display: flex;
      margin-top: 50px;
      width: 500px;
      flex-wrap: wrap;
    }

    &__select {
      padding: 15px 20px 15px 30px;
      margin-right: 30px;
      margin-bottom: 35px;
      width: 220px;
      height: 52px;
      border: 0.8px solid #AFB0B9;
      border-radius: 6px;
    }

    &__button {
      width: 152px;
    }
  }
</style>
