<template>
  <v-app>
    <Header />

    <v-main>
      <v-container>
        <nuxt />
      </v-container>
    </v-main>

    <Footer />
  </v-app>
</template>

<script>
import Header from '@/components/main/Header'
import Footer from '@/components/main/Footer'

export default {
  components: { Header, Footer },
}
</script>