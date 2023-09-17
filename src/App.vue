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
    <div class="calculator__section_bg"></div>
    <h3 class="calculator__section-title container">
      Увеличьте свой капитал <br> и достигайте финансовых вершин
    </h3>
    <div class="calculator__section-wrap">
      <div class="calculator__section-main--block-wrap">
      <div class="calculator__section-header">
        <h4 class="calculator__section-header--title">Выберите сумму и срок кредита</h4>
        <span class="calculator__section-header--steps">Шаг 1 из 4</span>
      </div>
      <div class="calculator__section-main--block">
        <h5 class="calculator__section-subheader">Желаемая сумма кредита</h5>
        <div class="calculator__section-sum" id="calc_sum">
          450 000 ₽
          <img src="/img/SVG.svg" alt="" class="calculator__section-edit--icon">
        </div>
        <input type="range" class="calculator__section-range" id="radius" min="50000" max="5000000">
        <div class="calculator__section-range--labels">
          <span class="calculator__section-range--label">50 000 ₽</span>
          <span class="calculator__section-range--label">300 000 ₽</span>
          <span class="calculator__section-range--label">1 000 000 ₽</span>
          <span class="calculator__section-range--label">5 000 000 ₽</span>
        </div>
        <div class="calculator__section-term--wrap">
          <div class="calculator__section-credit--term">
            <h5 class="calculator__section-subheader">Срок кредита</h5>
            <div class="calculator__section-sum calculator__section-date">
              5 лет
              <img src="/img/SVG.svg" alt="" class="calculator__section-edit--icon">
            </div>
            <input type="range" class="calculator__section-range calculator__section-range--date" id="radius" min="1" max="5">
            <div class="calculator__section-range--labels">
              <span class="calculator__section-range--label">1 год</span>
              <span class="calculator__section-range--label">5 лет</span>
            </div>
          </div>
          <div class="calculator__section-payment">
            <h5 class="calculator__section-subheader">Ежемесячный платеж</h5>
            <div class="calculator__section-sum" id="totalSum">
              9 650 ₽
            </div>
          </div>
        </div>
      </div>

      <select name="" id="" class="calc_target">
        <option value="" disabled selected>Цель кредита*</option>
        <option value="">Цель</option>
        <option value="">Цель</option>
      </select>

      <h4 class="calculator__section-header--title">Контактная информация</h4>
      <div class="calculator__contact_fio_wrap">
        <input type="text" class="calculator__contact_fio_input" placeholder="Фамилия, имя и отчество*">
        <div class="calculator__contact_fio_label">
          +20% к одобрению
        </div>
      </div>

      <div class="calc__fields_wrap">
        <input type="text" placeholder="Мобильный телефон*" class="calc_field">
        <input type="text" placeholder="Электронная почта" class="calc_field">
      </div>

      <div class="calc__footer">
        <hr>
        <div class="calc__footer-content--wrap">
          <span class="calc__footer-text">
            Заполняя форму, я принимаю
            <a href="#" class="calc__footer-link">условия передачи информации</a>
          </span>
          <a href="#" class="help__section-btn calc__footer_btn">Оформить</a>
        </div>
      </div>
      </div>

      <div class="calc__result_block">
        <div class="calc_result_wrap">
          <h5 class="calculator__section-subheader">
            Вы выбрали кредит на сумму
          </h5>
          <div class="calculator__section-sum" id="calc_sum"> 450 000 ₽</div>

          <h5 class="calculator__section-subheader calc__res_title">
            На срок
          </h5>
          <div class="calculator__section-sum" id="calc_sum"> 5 лет </div>

          <h5 class="calculator__section-subheader calc__res_title">
            Вероятность одобрения кредита
          </h5>
          <div class="calculator__section-sum" id="calc_sum"> 5% </div>

          <div class="calc_res__progress_bar">
            <div class="calc_res_bar__current"></div>
            <div class="calc_res_bar__plus"></div>
            <div class="calc_res_bar__place"></div>
          </div>
          <h5 class="calculator__section-subheader calc__plus_label">
            +50% за 1-й шаг
          </h5>
        </div>
      </div>
    </div>
  </section>
  <section class="steps container">
    <h3 class="calculator__section-title container steps__title">
      5 шагов <br>
      к получению инвестиций
    </h3>

    <div class="steps__wrap">
      <div class="step step__white">
        <span class="step_num step_num-black">01</span>
        <span class="step_title step_num-black">Оставляете <br> заявку</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="111" height="12" viewBox="0 0 111 12" fill="none">
          <path d="M111 6L101 0.226497V11.7735L111 6ZM0 7H102V5H0V7Z" fill="black"/>
        </svg>
      </div>
      <div class="step step__gray">
        <span class="step_num">02</span>
        <span class="step_title step_title-gray">Подготовка</span>
        <p class="step_description">
          Мы собираем необходимую информацию <br>
          о компании, проводим анализ данных, <br>
          выстраиваем стратегию работы.
        </p>
        <svg xmlns="http://www.w3.org/2000/svg" width="111" height="12" viewBox="0 0 111 12" fill="none">
          <path d="M111 6L101 0.226497V11.7735L111 6ZM0 7H102V5H0V7Z" fill="white"/>
        </svg>
      </div>
      <div class="step step__violet">
        <span class="step_num">03</span>
        <span class="step_title">Оставляете <br> заявку</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="111" height="12" viewBox="0 0 111 12" fill="none">
          <path d="M111 6L101 0.226497V11.7735L111 6ZM0 7H102V5H0V7Z" fill="white"/>
        </svg>
      </div>
      <div class="step step__green">
        <span class="step_num">04</span>
        <span class="step_title">Оставляете <br> заявку</span>
        <svg xmlns="http://www.w3.org/2000/svg" width="111" height="12" viewBox="0 0 111 12" fill="none">
          <path d="M111 6L101 0.226497V11.7735L111 6ZM0 7H102V5H0V7Z" fill="white"/>
        </svg>
      </div>
      <div class="step step__orange">
        <span class="step_num">05</span>
        <span class="step_title">Оставляете <br> заявку</span>
        <svg class="step_done" xmlns="http://www.w3.org/2000/svg" width="16" height="12" viewBox="0 0 16 12" fill="none">
          <path d="M5.32464 12C5.03844 12 4.76908 11.8896 4.56706 11.7004L0.307784 7.71145C0.0384222 7.45919 -0.0625883 7.09655 0.0384222 6.74968C0.139433 6.40282 0.425629 6.13478 0.796001 6.04018C1.16637 5.94558 1.55358 6.04018 1.82294 6.29245L5.29097 9.54039L14.1462 0.33263C14.3987 0.0645961 14.786 -0.0457708 15.1563 0.017296C15.5267 0.0961296 15.8297 0.348397 15.9476 0.679498C16.0654 1.02637 15.9812 1.389 15.7287 1.65703L6.13272 11.6531C5.9307 11.8581 5.66134 11.9685 5.37514 11.9842L5.32464 12Z" fill="white"/>
        </svg>
      </div>
    </div>
    <a href="#" class="help__section-btn steps_btn">Привлечь инвестиции</a>
  </section>

  <section class="wait">
    <div class="container">
    <h3 class="wait_title">Оставьте заявку <br>
      и ожидайте решения</h3>

    <div class="wait_table">
      <div class="wait_table-header wait_table-raw">
        <div class="wait_table-header--item">
          Дата
        </div>
        <div class="wait_table-header--item">
          Заемщик
        </div>
        <div class="wait_table-header--item">
          Сумма кредита
        </div>
        <div class="wait_table-header--item">
          Стадия
        </div>
        <div class="wait_table-header--item">
          Условия кредита
        </div>
      </div>
      <div class="wait_table-raw">
        <div class="wait_table-item">
          Сегодня
        </div>
        <div class="wait_table-item">
          Попов Н.Э.
        </div>
        <div class="wait_table-item">
          1 644 000₽
        </div>
        <div class="wait_table-item">
          Процедура андеррайтинга в банке
          <div class="wait_stage-wrap">
            <div class="wait_stage-item step__violet"></div>
            <div class="wait_stage-item step__green"></div>
            <div class="wait_stage-item step__orange"></div>
          </div>
        </div>
        <div class="wait_table-item">
          <div class="wait_terms">
            <div class="wait_terms-item">
              <div class="wait_terms-title">Банк</div>
              <div class="wait_terms-value">«СМП Банк»</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Одобренная сумма</div>
              <div class="wait_terms-value">1 355 000₽</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Еж. платеж</div>
              <div class="wait_terms-value">79 257₽</div>
            </div>
          </div>
        </div>
      </div>

      <div class="wait_table-raw">
        <div class="wait_table-item">
          Сегодня
        </div>
        <div class="wait_table-item">
          Попов Н.Э.
        </div>
        <div class="wait_table-item">
          1 644 000₽
        </div>
        <div class="wait_table-item">
          Процедура андеррайтинга в банке
          <div class="wait_stage-wrap">
            <div class="wait_stage-item step__violet"></div>
            <div class="wait_stage-item step__green"></div>
            <div class="wait_stage-item step__orange"></div>
          </div>
        </div>
        <div class="wait_table-item">
          <div class="wait_terms">
            <div class="wait_terms-item">
              <div class="wait_terms-title">Банк</div>
              <div class="wait_terms-value">«СМП Банк»</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Одобренная сумма</div>
              <div class="wait_terms-value">1 355 000₽</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Еж. платеж</div>
              <div class="wait_terms-value">79 257₽</div>
            </div>
          </div>
        </div>
      </div>

      <div class="wait_table-raw">
        <div class="wait_table-item">
          Сегодня
        </div>
        <div class="wait_table-item">
          Попов Н.Э.
        </div>
        <div class="wait_table-item">
          1 644 000₽
        </div>
        <div class="wait_table-item">
          Процедура андеррайтинга в банке
          <div class="wait_stage-wrap">
            <div class="wait_stage-item step__violet"></div>
            <div class="wait_stage-item step__green"></div>
            <div class="wait_stage-item step__orange"></div>
          </div>
        </div>
        <div class="wait_table-item">
          <div class="wait_terms">
            <div class="wait_terms-item">
              <div class="wait_terms-title">Банк</div>
              <div class="wait_terms-value">«СМП Банк»</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Одобренная сумма</div>
              <div class="wait_terms-value">1 355 000₽</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Еж. платеж</div>
              <div class="wait_terms-value">79 257₽</div>
            </div>
          </div>
        </div>
      </div>

      <div class="wait_table-raw">
        <div class="wait_table-item">
          Сегодня
        </div>
        <div class="wait_table-item">
          Попов Н.Э.
        </div>
        <div class="wait_table-item">
          1 644 000₽
        </div>
        <div class="wait_table-item">
          Процедура андеррайтинга в банке
          <div class="wait_stage-wrap">
            <div class="wait_stage-item step__violet"></div>
            <div class="wait_stage-item step__green"></div>
            <div class="wait_stage-item step__orange"></div>
          </div>
        </div>
        <div class="wait_table-item">
          <div class="wait_terms">
            <div class="wait_terms-item">
              <div class="wait_terms-title">Банк</div>
              <div class="wait_terms-value">«СМП Банк»</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Одобренная сумма</div>
              <div class="wait_terms-value">1 355 000₽</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Еж. платеж</div>
              <div class="wait_terms-value">79 257₽</div>
            </div>
          </div>
        </div>
      </div>

      <div class="wait_table-raw">
        <div class="wait_table-item">
          Сегодня
        </div>
        <div class="wait_table-item">
          Попов Н.Э.
        </div>
        <div class="wait_table-item">
          1 644 000₽
        </div>
        <div class="wait_table-item">
          Процедура андеррайтинга в банке
          <div class="wait_stage-wrap">
            <div class="wait_stage-item step__violet"></div>
            <div class="wait_stage-item step__green"></div>
            <div class="wait_stage-item step__orange"></div>
          </div>
        </div>
        <div class="wait_table-item">
          <div class="wait_terms">
            <div class="wait_terms-item">
              <div class="wait_terms-title">Банк</div>
              <div class="wait_terms-value">«СМП Банк»</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Одобренная сумма</div>
              <div class="wait_terms-value">1 355 000₽</div>
            </div>
            <div class="wait_terms-item">
              <div class="wait_terms-title">Еж. платеж</div>
              <div class="wait_terms-value">79 257₽</div>
            </div>
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
    return {}
  }
};
</script>
