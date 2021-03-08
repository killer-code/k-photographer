<template>
  <footer class="footer">
    <section class="app-container">
      <div class="footer__wrap my-16 pt-10">
        <div class="footer_top">
          <a href="/" class="logo">
            <img :src="require('@/assets/img/top-logo.svg')" alt="">
          </a>

          <ul class="anchor-list px-0">
            <li class="anchor mx-5 px-1">
              <a href="/" class="anchor__item">Главная</a>
            </li>
            <li class="anchor mx-5 px-1">
              <a href="/" class="anchor__item">Портфолио</a>
            </li>
            <li class="anchor mx-5 px-1">
              <a href="/" class="anchor__item">Цены</a>
            </li>
            <li class="anchor mx-5 px-1">
              <a href="/" class="anchor__item">Обо мне</a>
            </li>
            <li class="anchor mx-5 px-1">
              <a href="/" class="anchor__item">Отзывы</a>
            </li>
          </ul>

          <div class="contacts">
            <a href="" class="contacts__icon mx-1">
              <img :src="require('@/assets/img/icons/whatsup.svg')" alt="">
            </a>
            
            <a href="" class="contacts__icon mx-1">
              <img :src="require('@/assets/img/icons/insta.svg')" alt="">
            </a>

            <a href="">8 929 514 85 75</a>
          </div>
        </div>

        <div class="footer_bottom mt-10">
          <p class="mb-0">
            &copy;Катерина Татарова 2021
          </p>
          <p class="mb-0">
            г. Москва
          </p>
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style lang="scss" scoped>
.footer {
  font-size: 16px;
  line-height: 32px;
  color: #081A20;
  background-image: url('../../assets/img/copy-space-crumpled-white-paper.jpg');
  background-repeat: repeat;
  background-size: cover;

  &_top {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
  }

  &_bottom {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
  }
}

.anchor-list {
  display: flex;
  align-items: center;
  list-style-type: none;
}
.anchor {
  position: relative;
  ::before {
    content: '';
    position: absolute;
    width: 0;
    height: 1px;
    bottom: 0;
    left: 0;
    background-color: #019CFA;
    transition: all .5s ease;
  }
  :hover::before {  width: 100%; }

  &__item {
    font-size: 16px;
    line-height: 32px;
    color: #081A20;
    text-decoration: none;
    transition: all .5s ease;

    &:hover { color: #019CFA; }
  }
}

.contacts {
  display: flex;
  align-items: center;

  & a { 
    color: #081A20; 
    text-decoration: none;
  }
  &__icon {
    height: 20px;;
  }
}
</style>
