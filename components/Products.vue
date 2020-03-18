<template>
  <section id="awards" class="awards pb-70">
      <div class="container">
        <div class="row">
          <div class="col-sm-12 col-md-12 col-lg-10 offset-lg-1">
            <div class="heading heading-3 text-center mb-50">
              <span class="heading__subtitle">International standard company products</span>
              <h2 class="heading__title">We use High Quality certified products to our client installations</h2>
            </div><!-- /.heading -->
          </div><!-- /.col-lg-10 -->
        </div><!-- /.row -->
        <div class="row">
          <!-- feature item #1 -->
          <div class="col-sm-12 col-md-4 col-lg-4" v-for="(product, index) in products" :key="index">
            <div class="feature-item">
              <div class="feature__img">
                <img :src="product.image" alt="certificate" class="img-fluid">
              </div><!-- /.feature-img -->
              <div class="feature__content">
                <h4 class="feature__title">{{ product.title }}</h4>
                <p class="feature__desc">{{ product.desc }}</p>
              </div><!-- /.feature-content -->
            </div><!-- /.feature-item -->
          </div><!-- /.col-lg-4 -->
        </div><!-- /.row -->
      </div><!-- /.container -->
    </section><!-- /.awards -->
</template>

<script>
export default {
  props: ['products']
}
</script>