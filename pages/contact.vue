<template>
  <div>
     <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle :titleInfo="titleInfo" />
    <Contact />
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
import Contact from '@/components/Contact'
export default {
  head() {
    return {
      title: 'Contact Page',
      script: [{ src: '/js/main.js', ssr: true }]
    }
  },
  components: {
    Header,
    PageTitle,
    Contact
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