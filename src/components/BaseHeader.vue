<template>
  <header class="header">
    <div class="header__logo">
      <svg width="41" height="41" viewBox="0 0 41 41" fill="none" xmlns="http://www.w3.org/2000/svg">
        <circle cx="20.5" cy="20.5" r="20.5" fill="#1ABE84"/>
        <circle cx="20.5" cy="20.5" r="9" fill="#FB8F1D" stroke="white" stroke-width="3"/>
      </svg>
    </div>
    <div class="header__right-contain">
      <nav class="header__nav">
        <a href="#" class="header__nav-link">
          Home
        </a>
        <a href="#" class="header__nav-link">
          Destinations
        </a>
        <a href="#" class="header__nav-link">
          About
        </a>
        <a href="#" class="header__nav-link">
          Partner
        </a>
      </nav>
      <div class="header__active">
        <button class="header__active-button base-button base-button_border">
          Login
        </button>
        <button class="header__active-button base-button base-button_orange">
          Register
        </button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'BaseHeader',
};
</script>

<style lang="scss">
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 45px;

    &__right-contain {
      display: flex;
    }

    &__nav {
      display: flex;
      align-items: center;

      &-link {
        margin-right: 35px;
        color: #B8BECD;
        text-decoration:none;

        &:hover {
          color: #202336;
          font-weight: 500;
        }
      }
    }

    &__active {
      display: flex;

      &-button {
        width: 132px;
      }
    }
  }
</style>
