<template>
  <section id="slider1" class="slider slider-1">
      <div class="carousel owl-carousel carousel-arrows" data-slide="1" data-slide-md="1" data-slide-sm="1"
        data-autoplay="true" data-nav="true" data-dots="false" data-space="0" data-loop="true" data-speed="3000"
        data-transition="fade" data-animate-out="fadeOut" data-animate-in="fadeIn">
        <div class="slide-item align-v-h bg-overlay" v-for="(slider, index) in sliderData" :key="index">
          <div class="bg-img"><img :src="slider.img_url" alt="slide img"></div>
          <div class="container">
            <div class="row">
              <div class="col-sm-12 col-md-12 col-lg-8 col-xl-5" >
                <div class="slide__content">
                  <h2 class="slide__title">{{slider.title}}</h2>
                  <p class="slide__desc">{{slider.description}}</p>
                  <a :href="slider.btn_link" class="btn btn__white mr-40">{{slider.btn_text}}</a>
                  <a class="btn btn__video popup-video" href="https://www.youtube.com/watch?v=nrJtHemSPW4">
                    <div class="video__player">
                      <span class="video__player-animation"></span>
                      <span class="video__player-animation video__player-animation-2"></span>
                      <span class="video__player-animation video__player-animation-3"></span>
                      <i class="fa fa-play"></i>
                    </div>Our Video!
                  </a>
                </div><!-- /.slide-content -->
              </div><!-- /.col-xl-5 -->
              <div class="col-sm-12 col-md-12 col-lg-4 col-xl-3 offset-xl-4">
                <div class="slider__panel d-none d-lg-block">
                  <div class="slider__panel-icon">
                    <i :class="slider.panel_icon"></i>
                  </div>
                  <h3 class="slider__panel-title">{{slider.panel_title}}</h3>
                  <p class="slider__panel-desc">{{slider.panel_description}}
                  </p>
                  <a href="#" class="btn btn__primary btn__link">
                    <span>Explore</span>
                    <i class="icon-arrow-right2"></i>
                  </a>
                </div><!-- /.slider-panel -->
              </div><!-- /.col-xl-5 -->
            </div><!-- /.row -->
          </div><!-- /.container -->
        </div><!-- /.slide-item -->
      </div><!-- /.carousel -->
    </section><!-- /.slider -->
</template>

<script>
export default {
  props: ['sliderData']
}
</script>
