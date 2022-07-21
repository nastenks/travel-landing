<template>
  <div id="app">
    <BaseHeader />
    <MainBanner />
  </div>
</template>

<script>
import BaseHeader from './components/BaseHeader.vue';
import MainBanner from './components/MainBanner.vue';

export default {
  name: 'App',
  components: {
    BaseHeader, MainBanner,
  },
};
</script>

<style lang="scss">
  #app {
    font-family: Inter, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    max-width: 1140px;
    padding: 0 45px;
    margin: 0 auto;

    .base-button {
      display: flex;
      align-items: center;
      justify-content: center;
      border-radius: 8px;
      height: 44px;
      width: 132px;
      font-weight: 500;
      font-size: 15px;

      &_border {
        color: #FB8F1D;
        border: 1px solid #FB8F1D;
        background: none;
        margin-right: 18px;
      }

      &_orange {
        color: #FFFFFF;
        background: #FB8F1D;
        border: none;
      }
    }
  }
</style>
