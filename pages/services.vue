<template>
  <div>
     <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle :titleInfo="titleInfo" />
    <div class="container">
       <h2 class="heading__title text-center mt-4">Our Services</h2>
    </div>
    <About2 />
    <Clients :clients="clients" />
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
import About2 from '@/components/About2'
import Clients from '@/components/Clients'
export default {
  head() {
    return {
      title: 'Our Services',
      script: [{ src: '/js/main.js', difer: false, ssr: true }]
    }
  },
  components: {
    Header,
    PageTitle,
    About2,
    Clients
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
    clients: [
      {
        id: 1,
        image: '/images/clients/9.png',
        url: '#'
      },
      {
        id: 2,
        image: '/images/clients/10.png',
        url: '#'
      },
      {
        id: 3,
        image: '/images/clients/11.png',
        url: '#'
      },
      {
        id: 4,
        image: '/images/clients/12.png',
        url: '#'
      },
      {
        id: 5,
        image: '/images/clients/13.png',
        url: '#'
      },
      {
        id: 6,
        image: '/images/clients/14.png',
        url: '#'
      }
    ]
  })
}
</script>