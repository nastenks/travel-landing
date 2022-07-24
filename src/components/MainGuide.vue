<template>
  <section class="main-guide">
    <div class="main-guide__text">
      <h2 class="main-guide__text-title">
        Guides by Thousand Sunny
      </h2>
      <p class="main-guide__text-descr">
        Packed with tips and advice from our on-the-ground experts, our city guides app (iOS and Android) is the ultimate resource before and during a trip.
      </p>
      <button class="main-guide__text-button base-button base-button_orange">Download</button>
    </div>
    <div class="main-guide__image">
      <img src="/img/guide_image.png" alt="Picture on the guide" class="main-guide__image-man">
      <img src="/img/oval.svg" alt="Picture oval on the guide" class="main-guide__image-oval">
      <img src="/img/cross.svg" alt="Picture cross on the guide" class="main-guide__image-cross">
    </div>
  </section>
</template>

<script>
export default ({
  name: 'MainGuide',
})
</script>

<style lang="scss">
  .main-guide {
    margin-top: 390px;

    &__text {
      text-align: left;
      width: 450px;

      &-title {
        font-family: 'Playfair Display', sans-serif;
        font-weight: 700;
        font-size: 36px;
        line-height: 50px;
        color: #000000;
      }

      &-descr {
        font-family: 'Mulish', sans-serif;
        font-weight: 300;
        font-size: 17px;
        line-height: 30px;
        color: #7D7987;
      }

      &-button {
        margin-top: 40px;
        width: 164px;
        font-size: 16px;
      }
    }

    &__image {
      position: relative;

      &-man {
        position: absolute;
        width: 660px;
        left: 550px;
        bottom: -120px;
      }

      &-oval {
        position: absolute;
        width: 20px;
        left: 50px;
        top: -380px;
      }

      &-cross {
        position: absolute;
        transform: rotate(20deg);
        left: 420px;
        top: -15px;
      }
    }
  }
</style>
