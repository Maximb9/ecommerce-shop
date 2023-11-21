<script setup>
import { ref } from 'vue';

const menu = [
  {
    name: 'Plan pots',
    path: '/plant'
  },
  {
    name: 'Ceramics',
    path: '/plant'
  },
  {
    name: 'Tables',
    path: '/plant'
  },
  {
    name: 'Chairs',
    path: '/plant'
  },
  {
    name: 'Crockery',
    path: '/plant'
  },
  {
    name: 'Tableware',
    path: '/plant'
  },
  {
    name: 'Cutlery',
    path: '/plant'
  },
]
</script>

<template>
  <header class="header">
    <div class="header-top">
      <div class="header-top-search">
        <img src="/svg/Search.svg" alt="search">
      </div>
      <a href="#" class="header-logo">Avion</a>
      <div class="header-top-right">
        <div class="header-top-right__cart">
          <a href="#">
            <img src="/svg/Shopping--cart.svg" alt="">
          </a>
        </div>
        <div class="header-top-right__profile">
          <a href="#">
            <img src="/svg/User--avatar.svg" alt="profile">
          </a>
        </div>
      </div>
    </div>
    <div class="header-menu">
      <a
          class="header-menu__link"
          :href="element.path"
          v-for="(element, i) of menu"
          :key="i"
      >{{ element.name }}</a>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.header {
  height: 132px;
  background: #fff;

  &-top {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    justify-content: space-between;
    height: 70px;
    align-items: center;
    border-bottom: 1px solid rgba(0, 0, 0, .1);
    margin: 0 28px;
    &-right {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      &__cart {
        margin-right: 16px;
      }
    }
  }

  &-logo {
    color: #22202E;
    font-size: 24px;
    text-decoration: none;
    font-family: 'Clash Display', sans-serif;
    text-align: center;
    &:hover {
      text-decoration: underline;
    }
  }

  &-menu {
    height: 62px;
    display: flex;
    justify-content: center;
    align-items: center;
    &__link {
      margin: 0 22px;
      color: #726E8D;
      text-decoration: none;
      &:hover{
        text-decoration: underline;
      }
    }
  }
}
</style>