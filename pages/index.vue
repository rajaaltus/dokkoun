<template>
  <div>
    <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <Slider :sliderData="sliderData" />
    <Feature />
    <About />
    <Services />
    <Carousel />
    <Feature2 />
    <QuoteForm />
    <Testimonial />
  </div>
</template>

<script>
import Header from '@/components/Header'
import Slider from '@/components/Slider'
import Feature from '@/components/Feature'
import About from '@/components/About'
import Services from '@/components/Services'
import Carousel from '@/components/Carousel'
import Feature2 from '@/components/Feature2'
import QuoteForm from '@/components/QuoteForm'
import Testimonial from '@/components/Testimonial'
export default {
  head() {
    return {
      title: 'Dokkoun Sole Co., Ltd - Vientiane, Laos'
    }
  },
  layout: 'home',
  components: {
    Header,
    Slider,
    Feature,
    About,
    Services,
    Carousel,
    Feature2,
    QuoteForm,
    Testimonial
   
  },
  data: () => ({
    logo_url: '/images/logo/logo_square.svg',
    logo_dark_url: '/images/logo/logo_dark.png',
    sliderData: [
      {
        img_url: '/images/sliders/slider1.jpg',
        title: 'Industery Solutions!',
        description: 'To further develop our corporate strengths we have established a corporate mandate to maintain strong core values that truly reflect the companys philosophy.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-manufacturing-plant',
        panel_title: 'Our Mission',
        panel_description: 'Utilising latest processing solutions, and decades of work experience.',
      },
      {
        img_url: '/images/sliders/2.jpg',
        title: 'Reliable Effective',
        description: 'To further develop our corporate strengths we have established a corporate mandate to maintain strong core values that truly reflect the companys philosophy.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-wheel',
        panel_title: 'Our Vision',
        panel_description: 'Utilising latest processing solutions, and decades of work experience.',
      },
      {
        img_url: '/images/sliders/3.jpg',
        title: 'Safety & Integrity',
        description: 'To further develop our corporate strengths we have established a corporate mandate to maintain strong core values that truly reflect the companys philosophy.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-container',
        panel_title: 'Our Value',
        panel_description: 'Utilising latest processing solutions, and decades of work experience.',
      }
    ]
  })
}
</script>