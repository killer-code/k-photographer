<template>
  <section class="app-form-wrapper">
    <v-card class="card mt-16" width="500px" outlined shaped tile>
      <section class="card__header pa-6">
        <v-card-title class="pa-0">
          Авторизация
        </v-card-title>
      </section>
      <section class="card__body pa-6">

      </section>
    </v-card>
  </section>
</template>

<script>
export default {
  name: 'Login',
  layout: 'empty',
}
</script>

<style lang="scss" scoped>
.app-form-wrapper {
  display: flex;
  justify-content: center;
  height: 100vh;
}
.card {
  height: fit-content;
  &__header {
    background-color: #3e3e3e;
  }
}
</style>
