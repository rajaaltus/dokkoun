<template>
  <div>
    <Header :logo_url=logo_url :logo_dark_url=logo_dark_url />
    <div class="container">
    <nuxt />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'
export default {
  components: {
    Header,
    Footer
  },
  data: () => ({
    logo_url: '/images/logo/logo_square.svg',
    logo_dark_url: '/images/logo/logo_dark.png'
  })
}
</script>