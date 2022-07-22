<template>
  <section class="main-banner">
    <div class="main-banner__text">
      <h1 class="main-banner__title">Explore and <br> Travel</h1>
      <p class="main-banner__descr">Holiday finder</p>
      <form action="#" class="main-banner__form">
        <select id="check1" class="main-banner__select">
          <option value="Location">Location</option>
        </select>
        <select id="check2" class="main-banner__select">
          <option value="Activity">Activity</option>
        </select>
        <select id="3" class="main-banner__select">
          <option value="Grade">Grade</option>
        </select>
        <select id="4" class="main-banner__select">
          <option value="Date">Date</option>
        </select>
        <button class="main-banner__button base-button base-button_orange" type="submit">Explore</button>
      </form>
    </div>
    <div class="main-banner__image">
      <img src="/img/banner_image.png" alt="Picture on the banner" class="main-banner__image-man">
      <svg class="main-banner__image-cross" width="21" height="20" viewBox="0 0 21 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M13.6728 18.9121L12.7501 12.4686C12.7501 12.2176 12.9178 11.9665 13.1695 11.8828L19.6284 10.9624C19.88 10.9624 20.0478 10.7113 20.0478 10.3766L19.5445 6.77825C19.5445 6.5272 19.2928 6.35984 18.9573 6.35984L12.4984 7.28033C12.2467 7.28033 11.9951 7.11297 11.9113 6.86192L10.9885 0.41841C10.9885 0.167364 10.7369 0 10.4013 0L6.79442 0.502097C6.54277 0.502097 6.37501 0.753141 6.37501 1.08787L7.29774 7.53138C7.29774 7.78243 7.12998 8.03347 6.87833 8.11715L0.41941 9.03766C0.167764 9.03766 0 9.2887 0 9.62343L0.503271 13.2218C0.503271 13.4728 0.754928 13.6402 1.09046 13.6402L7.54938 12.7197C7.80102 12.7197 8.05268 12.887 8.13656 13.1381L9.05924 19.5816C9.05924 19.8326 9.3109 20 9.64643 20L13.2533 19.4979C13.505 19.4142 13.6728 19.1632 13.6728 18.9121Z" fill="#FDD08D"/>
      </svg>
      <svg class="main-banner__image-oval_bottom" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0.908711 14.1542C-1.39785 9.15663 0.846368 3.22201 5.83353 0.910617C10.8207 -1.40078 16.743 0.848123 19.0495 5.84573C21.3561 10.8433 19.1119 16.778 14.1247 19.0894C9.13753 21.4008 3.21528 19.1518 0.908711 14.1542ZM3.65165 12.9048C5.27248 16.4032 9.3869 17.9649 12.9403 16.3407C16.4313 14.7165 17.9898 10.5935 16.3689 7.03267C14.7481 3.47188 10.6337 1.9726 7.08033 3.59682C3.58931 5.22104 2.03082 9.40652 3.65165 12.9048Z" fill="url(#paint0_linear_1_889)"/>
        <defs>
          <linearGradient id="paint0_linear_1_889" x1="5.97093" y1="0.866138" x2="14.0704" y2="19.1436" gradientUnits="userSpaceOnUse">
            <stop stop-color="#BFF0DD"/>
            <stop offset="1" stop-color="#57D2A3"/>
          </linearGradient>
        </defs>
      </svg>
      <svg class="main-banner__image-oval_left" width="26" height="26" viewBox="0 0 26 26" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M1.18132 18.4005C-1.81721 11.9036 1.10028 4.18861 7.58359 1.1838C14.0669 -1.82101 21.7658 1.10256 24.7644 7.59945C27.7629 14.0963 24.8454 21.8114 18.3621 24.8162C11.8788 27.821 4.17986 24.8974 1.18132 18.4005ZM4.74714 16.7763C6.85422 21.3241 12.203 23.3544 16.8223 21.2429C21.3606 19.1314 23.3867 13.7715 21.2796 9.14248C19.1725 4.51345 13.8238 2.56438 9.20442 4.67587C4.6661 6.78736 2.64007 12.2285 4.74714 16.7763Z" fill="url(#paint0_linear_1_888)"/>
        <defs>
          <linearGradient id="paint0_linear_1_888" x1="7.76221" y1="1.12598" x2="18.2915" y2="24.8866" gradientUnits="userSpaceOnUse">
            <stop stop-color="#BFF0DD"/>
            <stop offset="1" stop-color="#57D2A3"/>
          </linearGradient>
        </defs>
      </svg>
    </div>
  </section>
</template>

<script>
export default ({
  name: 'MainBanner',
});
</script>

<style lang="scss">
  .main-banner {
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
