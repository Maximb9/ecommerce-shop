<script setup>

</script>

<template>
  <div class="hero">
    <img src="/img/Hero%20Blocks.jpg" alt="hero">
    <div class="hero-info">
      <div class="hero-info-text">
        <h2 class="hero-info__title">
          Luxury homeware for people who love timeless design quality
        </h2>
        <span class="hero-info__description">Shop the new Spring 2022 collection today</span>
      </div>
      <a href="#" class="hero-info-link">View collection</a>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.hero {
  height: 704px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  position: relative;

  &-img {
    max-width: 100%;
  }

  &-info {
    background: #fff;
    max-width: 630px;
    padding: 50px 55px;
    height: 444px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    margin-right: 80px;
    position: absolute;
    &__title{
     font-family: 'Clash Display', sans-serif;
      font-weight: 400;
      line-height: 1.5;
      margin: 0 0 20px 0;
    }
    &__description {
      color: #5B5676;
      font-size: 18px;
    }
    &-link {
      width: 170px;
      height: 56px;
      color: #2A254B;
      text-decoration: none;
      padding: 16px 32px;
      background: #F9F9F9;

      &:hover {
        text-decoration: none;

      }
    }
  }
}
</style>