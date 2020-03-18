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
      title: 'Dokkoun Sole Co., Ltd - Vientiane, Laos',
      script: [
        { src: '/js/main.js', difer: true },
      ]
    }
  },
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
        img_url: '/images/slider/slider1.jpg',
        title: 'Industery Solutions!',
        description: '20 Years of experience in providing Heavy Electrical work to various countries like South Korea, Japan and Laos.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-manufacturing-plant',
        panel_title: 'Our Mission',
        panel_description: 'We are committed to providing a quality service with a passion for electrical installation.',
      },
      {
        img_url: '/images/slider/slider2.jpg',
        title: 'Reliable Effective',
        description: 'Install all types of transformers or conversion pots plumbing and other construction installation activities. Electrical installation.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-wheel',
        panel_title: 'Our Vision',
        panel_description: 'Dokkhoun Sole Co., Ltd try to achieve a long term of electrical services and provide the quality of the services on electrical installation  to customers.',
      },
      {
        img_url: '/images/slider/slider3.jpg',
        title: 'Safety & Integrity',
        description: 'Our professional approach will provide solid Safety and integrity to achieve hassle-free electrical service.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-container',
        panel_title: 'Our Value',
        panel_description: 'Professional Approach, Experienced personnel, Committed to the quality.',
      },
      {
        img_url: '/images/slider/slider4.jpg',
        title: 'Safety & Secure',
        description: 'With the very long years of experience, we maintain the safety and security during the installation and after.',
        btn_link: '#',
        btn_text: 'Our Services',
        panel_icon: 'icon-container',
        panel_title: 'Our Value',
        panel_description: 'Professional Approach, Experienced personnel, Committed to the quality.',
      }
    ]
  })
}
</script>