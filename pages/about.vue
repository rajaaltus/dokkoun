<template>
  <div>
    <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle :titleInfo="titleInfo" />
    <About class="my-4" />
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
import About from '@/components/About'
export default {
  head() {
    return {
      title: 'About Page',
      script: [{ src: '/js/main.js', difer: true, ssr: true }]
    }
  },
  components: {
    Header,
    PageTitle,
    About
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