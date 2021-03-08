<template>
  <nav class="app-container navigation py-4">
    <v-row class="wrap align-center mx-0">
      <a href="/">
        <img :src="require('@/assets/img/top-logo.svg')" alt="">
      </a>

      <ul class="anchor-list">
        <li class="anchor mr-10 px-1">
          <a href="/" class="anchor__item">Главная</a>
        </li>
        <li class="anchor mr-10 px-1">
          <a href="/" class="anchor__item">Портфолио</a>
        </li>
        <li class="anchor mr-10 px-1">
          <a href="/" class="anchor__item">Цены</a>
        </li>
        <li class="anchor mr-10 px-1">
          <a href="/" class="anchor__item">Обо мне</a>
        </li>
        <li class="anchor mr-10 px-1">
          <a href="/" class="anchor__item">Отзывы</a>
        </li>
      </ul>
    </v-row>

    <section class="contact">
      <div class="contact_top">
        <p class="mb-0">г.Москва</p>
      </div>

      <div class="contact_bottom">
        <div class="social">
          <a href=""><img :src="require('@/assets/img/icons/whatsup.svg')" alt=""></a>
          <a href=""><img :src="require('@/assets/img/icons/insta.svg')" alt=""></a>
        </div>

        <div class="phone">
          <a href="">8 929 514 85 75</a>
        </div>
      </div>
    </section>
  </nav>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style lang="scss" scoped>
.navigation {
  display: flex;
  align-items: center;
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
    background-color: #183D47;
    transition: all .5s ease;
  }
  :hover::before {  width: 100%; }

  &__item {
    font-size: 16px;
    line-height: 32px;
    color: #fff;
    text-decoration: none;
    transition: all .5s ease;

    &:hover { color: #019CFA; }
  }
}

.contact {
  &_bottom {
    display: flex;

    & a { 
      color: #fff;
      text-decoration: none; 
    }
  }
}
</style>
