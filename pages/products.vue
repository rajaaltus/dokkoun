<template>
  <div>
     <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle :titleInfo="titleInfo" />
    <Products :products="products" />
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
import Products from '@/components/Products'
export default {
  head() {
    return {
      title: 'Our Products',
      script: [{ src: '/js/main.js', difer: true, ssr: true }]
    }
  },
  components: {
    Header,
    PageTitle,
    Products
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
    products: [
    {
      id: 1,
      image: '/images/products/1.png',
      title: 'Line Post',
      desc: 'Medium voltage composite polymeric post type insulators from China manufacturer.'
    },
    {
      id: 2,
      image: '/images/products/2.png',
      title: 'Drop-Down Switch',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    },
    {
      id: 3,
      image: '/images/products/3.jpg',
      title: 'Family Business Award',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    },
    {
      id: 4,
      image: '/images/products/4.jpg',
      title: 'Family Business Award',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    },
    {
      id: 5,
      image: '/images/products/5.jpg',
      title: 'Family Business Award',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    },
    {
      id: 6,
      image: '/images/products/6.jpg',
      title: 'Family Business Award',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    },
    {
      id: 7,
      image: '/images/products/1.jpg',
      title: 'Family Business Award',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    },
    {
      id: 8,
      image: '/images/products/2.jpg',
      title: 'Family Business Award',
      desc: 'We believe that partnerships are fundamental to our growth. We\'ll seek the highest quality global forwarding services.'
    }
  ]
  })
}
</script>