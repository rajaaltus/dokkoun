<template>
  <div>
    <Header />
    <Slider />
    <Feature />
    <About />
    <Services />
    <Carousel />
    <Feature2 />
    <QuoteForm />
    <Testimonial />
    <Footer />
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
import Footer from '@/components/Footer'
export default {
  head() {
    return {
      title: 'Dokkoun Sole Co., Ltd - Vientiane, Laos'
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
    Testimonial,
    Footer
  }
}
</script>