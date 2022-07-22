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
    <ul class="main-gallery__list">
      <li class="main-gallery__list-item" v-for="item in randomCountries" :key="item.id">
        <figure>
          <img :src="item.image" :alt="item.title">
          <figcaption>
            <b>
              {{ item.title }}
            </b>
            <p>
              {{ item.country }}
            </p>
          </figcaption>
        </figure>
      </li>
    </ul>
  </section>
</template>

<script>
import countries from '../data/countries';

export default ({
  name: 'MainGallery',
  data() {
    return {
      countries,
    };
  },
  computed: {
    randomCountries() {
      const randArray = countries.sort(() => 0.5 - Math.random());
      let resArray = randArray.slice(0, 4);
      return resArray;
    },
  },
});
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

    &__list {
      display: flex;
      justify-content: space-between;

      &-item {
        list-style-type: none;
        width: 260px;
        height: 332px;
        overflow: hidden;

        img {
          height: 332px;
        }
      }
    }

    ul,
    figure {
      padding: 0;
      margin: 0;
    }
  }
</style>
