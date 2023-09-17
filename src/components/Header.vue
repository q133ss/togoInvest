<script setup>

</script>

<template>
<nav class="header__nav container">
  <div class="header__left-wrap">
  <span class="logo__text">
    TOGO
    <span class="logo__primary-text">
      invest
    </span>
  </span>

  <ul class="menu">
    <li class="header__menu-item">
      Инвесторам
    </li>
    <li class="header__menu-item">
      Партнерам
    </li>
    <li class="header__menu-item">
      Контакты
    </li>
  </ul>
  </div>
  <div class="header__phone">
    <img src="/img/Phone.png" alt="" class="header__phone-img">
    <a href="tel:+62123412008" class="header__phone-text">+62 123-412-008</a>
  </div>
  <div class="mob_menu" @click="mobMenu()">
    <svg xmlns="http://www.w3.org/2000/svg" x="0px" y="0px" width="64" height="64" viewBox="0 0 72 72"
         style="fill:#FFFFFF;">
      <path d="M56 48c2.209 0 4 1.791 4 4 0 2.209-1.791 4-4 4-1.202 0-38.798 0-40 0-2.209 0-4-1.791-4-4 0-2.209 1.791-4 4-4C17.202 48 54.798 48 56 48zM56 32c2.209 0 4 1.791 4 4 0 2.209-1.791 4-4 4-1.202 0-38.798 0-40 0-2.209 0-4-1.791-4-4 0-2.209 1.791-4 4-4C17.202 32 54.798 32 56 32zM56 16c2.209 0 4 1.791 4 4 0 2.209-1.791 4-4 4-1.202 0-38.798 0-40 0-2.209 0-4-1.791-4-4 0-2.209 1.791-4 4-4C17.202 16 54.798 16 56 16z"></path>
    </svg>
  </div>
</nav>

<div class="mobile_menu-wrap" :class="{open: isActive}">
<nav>
  <a href="#" id="close_menu" @click="close">X</a>
  <ul class="mobile_menu_list">
    <li class="mobile__menu-item">
      <a href="#">Инвесторам</a>
    </li>
    <li class="mobile__menu-item">
      <a href="#">Партнерам</a>
    </li>
    <li class="mobile__menu-item">
      <a href="#">Контакты</a>
    </li>
  </ul>
</nav>
</div>

</template>

<style scoped>
</style>

<script>
export default {
  data() {
    return {
      isActive: false
    }
  },
  methods:{
    mobMenu: function (){
      this.isActive = !this.isActive;
    },
    close: function (){
      this.isActive = false;
    }
  }
}
</script>