<template>
  <div>
     <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle :titleInfo="titleInfo" />
    <h1>Our Products</h1>
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
export default {
  head() {
    return {
      title: 'Our Portfolio',
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
    titleInfo: 
    { 
      img_url: '/images/sliders/slider1.jpg',
      subTitle: 'Building The Future, Restoring The Past',
      title: 'Individually Assess Each Plan & Offer Optimal Solutions!'
    },
  })
}
</script>