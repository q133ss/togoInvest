<script setup>
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
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

  <section class="programs container">
    <div class="programs_header">
      <h3 class="programs_title">
        Кредитные программы
      </h3>
      <div class="programs_selector">
        <span class="programs_selector-item active">
          Кампаниям
        </span>
        <span class="programs_selector-item">
          ИП
        </span>
        <span class="programs_selector-item">
          Физическим лицам
        </span>
      </div>
    </div>

    <div class="programs_wrap">
      <div class="program">
        <div class="program_wrap">
        <div class="program_header">
          <h4 class="program_title">
            Экспресс кредит
          </h4>
          <span class="program_bid">
            от 4.4%
            <span class="program_bid_old">
              от 15%
            </span>
          </span>

          <div class="program_terms">
            <span class="program_term_title">
              Условия получения
            </span>
            <span class="program_term">Компании более года</span>
            <span class="program_term">Нет текущих просрочек</span>
            <span class="program_term">Без обеспечения</span>
          </div>
        </div>
        <div class="program_body">
          <div class="program_item">
            <div class="program_item-title">
              Сумма кредита
            </div>

            <div class="program_item-price">
              1 000 000 - 15 000 000 ₽
            </div>

            <div class="program_item-subtitle">
              онлайн-решение за 1 минуту
            </div>
          </div>

          <div class="program_item">
            <div class="program_item-title">
              Срок кредита
            </div>

            <div class="program_item-price">
              до 5 лет
            </div>

            <div class="program_item-subtitle">
              с возможностью досрочного погашения
            </div>
          </div>

          <div class="program_item">
            <div class="program_item-title">
              Бесплатно
            </div>

            <div class="program_item-insurance">
              <svg xmlns="http://www.w3.org/2000/svg" width="31" height="30" viewBox="0 0 31 30" fill="none">
                <path d="M15.4578 28.0828C8.24375 28.0828 2.375 22.2141 2.375 15C2.375 7.78592 8.24375 1.91718 15.4578 1.91718C17.5813 1.91718 19.6887 2.43749 21.5544 3.42093C22.2388 3.7828 22.5012 4.6303 22.1403 5.31561C21.7794 6.00093 20.9328 6.26343 20.2456 5.90155C18.7822 5.12905 17.1266 4.72124 15.4578 4.72124C9.78969 4.72124 5.17812 9.33186 5.17812 15C5.17812 20.6681 9.78875 25.2787 15.4569 25.2787C21.125 25.2787 25.7366 20.6681 25.7366 15C25.7366 14.3522 25.6766 13.7044 25.5575 13.0772C25.4131 12.3169 25.9128 11.5828 26.6731 11.4384C27.4334 11.2931 28.1675 11.7947 28.3109 12.5541C28.4628 13.3537 28.5397 14.1759 28.5397 14.9991C28.5406 22.2141 22.6709 28.0828 15.4578 28.0828Z" fill="#52A516"/>
                <path d="M14.0956 20.1684C13.7244 20.1684 13.3662 20.0194 13.1028 19.7569L9.15875 15.8006C8.61218 15.2522 8.61406 14.3653 9.16156 13.8178C9.71 13.2712 10.5969 13.2722 11.1444 13.8206L14.0975 16.7831L26.2325 4.65187C26.78 4.10437 27.6678 4.10437 28.2153 4.65187C28.7619 5.19937 28.7619 6.08718 28.2153 6.63374L15.0875 19.7587C14.8241 20.0203 14.4669 20.1684 14.0956 20.1684Z" fill="#52A516"/>
              </svg>
              Отказ от страховки
            </div>

            <div class="program_item-subtitle">
              экономия до 30% от суммы кредита
            </div>
          </div>
        </div>
        </div>
        <a href="#" class="help__section-btn program_btn">Получить кредит</a>
      </div>

      <div class="program">
        <div class="program_wrap">
          <div class="program_header">
            <h4 class="program_title">
              Экспресс кредит
            </h4>
            <span class="program_bid">
            от 4.4%
            <span class="program_bid_old">
              от 15%
            </span>
          </span>

            <div class="program_terms">
            <span class="program_term_title">
              Условия получения
            </span>
              <span class="program_term">Компании более года</span>
              <span class="program_term">Нет текущих просрочек</span>
              <span class="program_term">Без обеспечения</span>
            </div>
          </div>
          <div class="program_body">
            <div class="program_item">
              <div class="program_item-title">
                Сумма кредита
              </div>

              <div class="program_item-price">
                1 000 000 - 15 000 000 ₽
              </div>

              <div class="program_item-subtitle">
                онлайн-решение за 1 минуту
              </div>
            </div>

            <div class="program_item">
              <div class="program_item-title">
                Срок кредита
              </div>

              <div class="program_item-price">
                до 5 лет
              </div>

              <div class="program_item-subtitle">
                с возможностью досрочного погашения
              </div>
            </div>

            <div class="program_item">
              <div class="program_item-title">
                Бесплатно
              </div>

              <div class="program_item-insurance">
                <svg xmlns="http://www.w3.org/2000/svg" width="31" height="30" viewBox="0 0 31 30" fill="none">
                  <path d="M15.4578 28.0828C8.24375 28.0828 2.375 22.2141 2.375 15C2.375 7.78592 8.24375 1.91718 15.4578 1.91718C17.5813 1.91718 19.6887 2.43749 21.5544 3.42093C22.2388 3.7828 22.5012 4.6303 22.1403 5.31561C21.7794 6.00093 20.9328 6.26343 20.2456 5.90155C18.7822 5.12905 17.1266 4.72124 15.4578 4.72124C9.78969 4.72124 5.17812 9.33186 5.17812 15C5.17812 20.6681 9.78875 25.2787 15.4569 25.2787C21.125 25.2787 25.7366 20.6681 25.7366 15C25.7366 14.3522 25.6766 13.7044 25.5575 13.0772C25.4131 12.3169 25.9128 11.5828 26.6731 11.4384C27.4334 11.2931 28.1675 11.7947 28.3109 12.5541C28.4628 13.3537 28.5397 14.1759 28.5397 14.9991C28.5406 22.2141 22.6709 28.0828 15.4578 28.0828Z" fill="#52A516"/>
                  <path d="M14.0956 20.1684C13.7244 20.1684 13.3662 20.0194 13.1028 19.7569L9.15875 15.8006C8.61218 15.2522 8.61406 14.3653 9.16156 13.8178C9.71 13.2712 10.5969 13.2722 11.1444 13.8206L14.0975 16.7831L26.2325 4.65187C26.78 4.10437 27.6678 4.10437 28.2153 4.65187C28.7619 5.19937 28.7619 6.08718 28.2153 6.63374L15.0875 19.7587C14.8241 20.0203 14.4669 20.1684 14.0956 20.1684Z" fill="#52A516"/>
                </svg>
                Отказ от страховки
              </div>

              <div class="program_item-subtitle">
                экономия до 30% от суммы кредита
              </div>
            </div>
          </div>
        </div>
        <a href="#" class="help__section-btn program_btn">Получить кредит</a>
      </div>

      <div class="program">
        <div class="program_wrap">
          <div class="program_header">
            <h4 class="program_title">
              Экспресс кредит
            </h4>
            <span class="program_bid">
            от 4.4%
            <span class="program_bid_old">
              от 15%
            </span>
          </span>

            <div class="program_terms">
            <span class="program_term_title">
              Условия получения
            </span>
              <span class="program_term">Компании более года</span>
              <span class="program_term">Нет текущих просрочек</span>
              <span class="program_term">Без обеспечения</span>
            </div>
          </div>
          <div class="program_body">
            <div class="program_item">
              <div class="program_item-title">
                Сумма кредита
              </div>

              <div class="program_item-price">
                1 000 000 - 15 000 000 ₽
              </div>

              <div class="program_item-subtitle">
                онлайн-решение за 1 минуту
              </div>
            </div>

            <div class="program_item">
              <div class="program_item-title">
                Срок кредита
              </div>

              <div class="program_item-price">
                до 5 лет
              </div>

              <div class="program_item-subtitle">
                с возможностью досрочного погашения
              </div>
            </div>

            <div class="program_item">
              <div class="program_item-title">
                Бесплатно
              </div>

              <div class="program_item-insurance">
                <svg xmlns="http://www.w3.org/2000/svg" width="31" height="30" viewBox="0 0 31 30" fill="none">
                  <path d="M15.4578 28.0828C8.24375 28.0828 2.375 22.2141 2.375 15C2.375 7.78592 8.24375 1.91718 15.4578 1.91718C17.5813 1.91718 19.6887 2.43749 21.5544 3.42093C22.2388 3.7828 22.5012 4.6303 22.1403 5.31561C21.7794 6.00093 20.9328 6.26343 20.2456 5.90155C18.7822 5.12905 17.1266 4.72124 15.4578 4.72124C9.78969 4.72124 5.17812 9.33186 5.17812 15C5.17812 20.6681 9.78875 25.2787 15.4569 25.2787C21.125 25.2787 25.7366 20.6681 25.7366 15C25.7366 14.3522 25.6766 13.7044 25.5575 13.0772C25.4131 12.3169 25.9128 11.5828 26.6731 11.4384C27.4334 11.2931 28.1675 11.7947 28.3109 12.5541C28.4628 13.3537 28.5397 14.1759 28.5397 14.9991C28.5406 22.2141 22.6709 28.0828 15.4578 28.0828Z" fill="#52A516"/>
                  <path d="M14.0956 20.1684C13.7244 20.1684 13.3662 20.0194 13.1028 19.7569L9.15875 15.8006C8.61218 15.2522 8.61406 14.3653 9.16156 13.8178C9.71 13.2712 10.5969 13.2722 11.1444 13.8206L14.0975 16.7831L26.2325 4.65187C26.78 4.10437 27.6678 4.10437 28.2153 4.65187C28.7619 5.19937 28.7619 6.08718 28.2153 6.63374L15.0875 19.7587C14.8241 20.0203 14.4669 20.1684 14.0956 20.1684Z" fill="#52A516"/>
                </svg>
                Отказ от страховки
              </div>

              <div class="program_item-subtitle">
                экономия до 30% от суммы кредита
              </div>
            </div>
          </div>
        </div>
        <a href="#" class="help__section-btn program_btn">Получить кредит</a>
      </div>
    </div>
  </section>

  <section class="coop">
    <div class="container">
    <h3 class="wait_title">
      Сотрудничаем с 19 банками и 6 <br>
      краундлендинговыми платформами
    </h3>

    <div class="coop_wrap">
      <div class="coop_item">
        <img src="/img/Sber Avto logo 1.png" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/tochka-bank_logo 1.png" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/Group 956.svg" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/PochtaBank logo 1.svg" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/finam_logo 1.png" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/Sber Avto logo 1.png" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/tochka-bank_logo 1.png" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/Group 956.svg" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/PochtaBank logo 1.svg" alt="">
      </div>

      <div class="coop_item">
        <img src="/img/finam_logo 1.png" alt="">
      </div>
    </div>
    </div>
  </section>

  <section class="history container">
    <h3 class="programs_title">истории наших клиентов</h3>

    <div class="history_wrap">
      <div class="history_btns">
        <div class="history_left_btn history_btn" @click="prevSlide">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 16 16" fill="none">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M3.9332 9.1L9.01431 14.1811L7.6001 15.5953L0.104797 8.1L7.6001 0.604697L9.01431 2.0189L3.9332 7.1L15.0954 7.1L15.0954 9.1L3.9332 9.1Z" fill="#10273D" fill-opacity="0.3"/>
          </svg>
        </div>

        <div class="history_right_btn history_btn" @click="nextSlide">
          <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 16 16" fill="none">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M12.0668 6.9L6.98566 1.81888L8.39987 0.404663L15.8952 7.9L8.39987 15.3953L6.98566 13.9811L12.0668 8.9H0.904541V6.9H12.0668Z" fill="#40AB91"/>
          </svg>
        </div>
      </div>

      <swiper
          :slides-per-view="2"
          :space-between="28"
          @swiper="onSwiper"
      >
        <swiper-slide>
          <div class="history_slider_wrap">
            <p class="history_text">
              Основатель сервиса по продвижению на маркетплейсах MPLAB,  10 тыс. + пользователей.Александр обратился с запросом привлечения инвестиций в свою IT компанию.По факту проделанной работы через 3 дня мы привлекли Александру 5 миллионов рублей и взаимодействуем далее, выстроили долгосрочную стратегию по привлечению средств.
            </p>
            <div class="history_author-wrap">
              <span class="history_author">
                Павел
              </span>
              <span class="history_job">
                ИП в сфере дистрибуции
              </span>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="history_slider_wrap">
            <p class="history_text">
              Основатель сервиса по продвижению на маркетплейсах MPLAB,  10 тыс. + пользователей.Александр обратился с запросом привлечения инвестиций в свою IT компанию.По факту проделанной работы через 3 дня мы привлекли Александру 5 миллионов рублей и взаимодействуем далее, выстроили долгосрочную стратегию по привлечению средств.
            </p>

            <div class="history_author-wrap">
              <span class="history_author">
                Павел
              </span>
              <span class="history_job">
                ИП в сфере дистрибуции
              </span>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="history_slider_wrap">
            <p class="history_text">
              Основатель сервиса по продвижению на маркетплейсах MPLAB,  10 тыс. + пользователей.Александр обратился с запросом привлечения инвестиций в свою IT компанию.По факту проделанной работы через 3 дня мы привлекли Александру 5 миллионов рублей и взаимодействуем далее, выстроили долгосрочную стратегию по привлечению средств.
            </p>
            <div class="history_author-wrap">
              <span class="history_author">
                Павел
              </span>
              <span class="history_job">
                ИП в сфере дистрибуции
              </span>
            </div>
          </div>
        </swiper-slide>

        <swiper-slide>
          <div class="history_slider_wrap">
            <p class="history_text">
              Основатель сервиса по продвижению на маркетплейсах MPLAB,  10 тыс. + пользователей.Александр обратился с запросом привлечения инвестиций в свою IT компанию.По факту проделанной работы через 3 дня мы привлекли Александру 5 миллионов рублей и взаимодействуем далее, выстроили долгосрочную стратегию по привлечению средств.
            </p>
            <div class="history_author-wrap">
              <span class="history_author">
                Павел
              </span>
              <span class="history_job">
                ИП в сфере дистрибуции
              </span>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </section>
  <Footer></Footer>
</template>
<style scoped>
</style>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  mounted() {

  },
  setup() {

  },
  data() {
    return {
      swiper: null,
    };
  },
  methods: {
    onSwiper(swiper) {
      this.swiper = swiper;
    },

    nextSlide() {
      this.swiper.slideNext()
    },
    prevSlide() {
      this.swiper.slidePrev()
    }
  },
};
</script>
