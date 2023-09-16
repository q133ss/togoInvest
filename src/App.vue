<script setup>
import Header from "./components/Header.vue";
</script>

<template>
  <section class="main__section">
    <Header></Header>
    <div class="main__screen-content">
      <div class="main__screen-content--wrap container">
        <h1 class="main__screen-content--title">
          Увеличьте свой капитал и достигайте финансовых вершин
        </h1>
        <div class="main__screen-content--description-wrap">
          <div class="main__screen-content--rectangle"></div>
          <div class="main__screen-content--description">
          Наша команда — группа экспертов <br>
          по привлечению инвестиций для развития вашего дела.
          </div>
        </div>
        <a href="#" class="main__screen-btn">
          Привлечь инвестиции
        </a>
      </div>
    </div>
  </section>
  <section class="help__section container">
    <img src="/img/help.png" alt="" class="help__section-img">
    <div class="help__section-content">
      <h3 class="help__section-title">Качественная и быстрая помощь в привлечении инвестиций для вашего бизнеса</h3>
      <p class="help__section-text">
        Наша компания - это профессиональный и надежный партнер для всех, кому необходимо привлечь инвестиции и кредитование в банках.   Мы предоставляем широкий спектр инвестиционных услуг и консультаций, которые помогают нашим клиентам принимать получать максимально выгодные одобрения.
        Мы постоянно совершенствуем свои знания и навыки, чтобы быть в курсе всех изменений на рынке и предлагать нашим клиентам наиболее эффективные инвестиционные решения.
      </p>
      <a href="#" class="help__section-btn">Привлечь инвестиции</a>
    </div>
  </section>
  <section class="calculator__section">
    <h3 class="calculator__section-title container">
      Увеличьте свой капитал <br> и достигайте финансовых вершин
    </h3>
    <div class="calculator__section-wrap">
      <div class="calculator__section-header">
        <h4 class="calculator__section-header--title">Выберите сумму и срок кредита</h4>
        <span class="calculator__section-header--steps">Шаг 1 из 4</span>
      </div>
      <div class="calculator__section-main--block">
        <h5 class="calculator__section-subheader">Желаемая сумма кредита</h5>
        <div class="calculator__section-sum">
          450 000 ₽
          <img src="/img/SVG.svg" alt="" class="calculator__section-edit--icon">
        </div>
        <input type="range" class="calculator__section-range" id="radius" min="50000" max="5000000">
<!--         тут лейблы -->
        <div class="calculator__section-term--wrap">
          <div class="calculator__section-credit--term">
            <h5>Срок кредита</h5>
            <div class="calculator__section-sum">
              5 лет
              <img src="/img/SVG.svg" alt="" class="calculator__section-edit--icon">
            </div>
            <input type="range" class="calculator__section-range" id="radius" min="1" max="5">
          </div>
          <div class="calculator__section-payment">
            <h5 class="calculator__section-subheader">Ежемесячный платеж</h5>
            <div class="calculator__section-sum">
              9 650 ₽
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
</style>
<script>
export default {
  data() {
    return {
      value: 1
    }
  }
};
</script>
