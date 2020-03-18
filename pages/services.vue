<template>
  <div>
     <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle />
    <h1>Our Services</h1>
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
export default {
  head() {
    return {
      title: 'Our Services',
      script: [{ src: '/js/main.js', difer: false, ssr: true }]
    }
  },
  components: {
    Header,
    PageTitle
  },
  data: () => ({
    logo_url: '/images/logo/logo_square.svg',
    logo_dark_url: '/images/logo/logo_dark.png',
  })
}
</script>