<template>
  <section class="main-promo">
    <div class="main-promo__image">
      <img src="/img/promo_image.png" alt="Picture on the banner" class="main-promo__image-man">
      <svg class="main-promo__image-oval" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0.908711 14.1542C-1.39785 9.15663 0.846368 3.22201 5.83353 0.910617C10.8207 -1.40078 16.743 0.848123 19.0495 5.84573C21.3561 10.8433 19.1119 16.778 14.1247 19.0894C9.13753 21.4008 3.21528 19.1518 0.908711 14.1542ZM3.65165 12.9048C5.27248 16.4032 9.3869 17.9649 12.9403 16.3407C16.4313 14.7165 17.9898 10.5935 16.3689 7.03267C14.7481 3.47188 10.6337 1.9726 7.08033 3.59682C3.58931 5.22104 2.03082 9.40652 3.65165 12.9048Z" fill="url(#paint0_linear_1_910)"/>
        <defs>
          <linearGradient id="paint0_linear_1_910" x1="5.97093" y1="0.866138" x2="14.0704" y2="19.1436" gradientUnits="userSpaceOnUse">
            <stop stop-color="#BFF0DD"/>
            <stop offset="1" stop-color="#57D2A3"/>
          </linearGradient>
        </defs>
      </svg>
      <svg class="main-promo__image-cross" width="21" height="21" viewBox="0 0 21 21" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M12.698 19.5325L12.6228 13.0237C12.6555 12.7748 12.8545 12.5478 13.1149 12.4976L19.6387 12.4266C19.8882 12.4594 20.0872 12.2323 20.1308 11.9004L20.1007 8.26722C20.1335 8.01832 19.9058 7.81959 19.5731 7.77587L13.0493 7.84688C12.7998 7.81408 12.5721 7.61536 12.5217 7.35553L12.4464 0.846713C12.4792 0.597808 12.2515 0.399078 11.9188 0.355357L8.2772 0.38317C8.0277 0.350379 7.82866 0.577422 7.78504 0.909296L7.86028 7.41811C7.82756 7.66701 7.62852 7.89406 7.36811 7.94423L0.844312 8.01526C0.594812 7.98247 0.395766 8.20951 0.352149 8.54138L0.382245 12.1746C0.349532 12.4235 0.577234 12.6222 0.909901 12.666L7.4337 12.5949C7.6832 12.6277 7.9109 12.8265 7.96136 13.0863L8.03654 19.5951C8.00383 19.844 8.23153 20.0427 8.5642 20.0865L12.2058 20.0587C12.4662 20.0085 12.6652 19.7814 12.698 19.5325Z" fill="#FDD08D"/>
      </svg>
    </div>
    <div class="main-promo__text">
      <h2 class="main-promo__text-title">A new way to explore the world</h2>
      <p class="main-promo__text-descr">For decades travellers have reached for Lonely Planet books when looking to plan and execute their perfect trip, but now, they can also let Lonely Planet Experiences lead the way</p>
      <button class="main-promo__text-button base-button base-button_orange">Learn more</button>
    </div>
  </section>
</template>

<script>
export default ({
  name: 'MainPromo',
});
</script>

<style lang="scss">
  .main-promo {
    display: flex;
    margin-top: 286px;
    justify-content: flex-end;

    &__text {
      margin-top: 95px;
      width: 450px;
      text-align: left;

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
        margin-top: 22px;
        width: 164px;
        font-size: 16px;
      }
    }

    &__image {
      position: relative;

      &-man {
        position: absolute;
        width: 660px;
        left: -750px;
        top: 0;
      }

      &-oval {
        position: absolute;
        left: 320px;
        top: 390px;
      }

      &-cross {
        position: absolute;
        left: -80px;
        top: -30px;
      }
    }
  }
</style>
