<template>
   <section id="pageTitle" class="page-title bg-overlay bg-parallax">
      <div class="bg-img"><img :src="titleInfo.img_url" alt="background"></div>
      <div class="container">
        <div class="row">
          <div class="col-sm-12 col-md-12 col-lg-12 col-xl-8">
            <span class="pagetitle__subheading">{{titleInfo.subTitle}}</span>
            <h1 class="pagetitle__heading">{{titleInfo.title}}</h1>
            <nav aria-label="breadcrumb">
              <ol class="breadcrumb">
                <li class="breadcrumb-item"><a href="#">Home</a></li>
                <li class="breadcrumb-item"><a href="#">Company</a></li>
                <li class="breadcrumb-item active" aria-current="page">About Us</li>
              </ol>
            </nav>
          </div><!-- /.col-xl-8 -->
        </div><!-- /.row -->
      </div><!-- /.container -->
    </section><!-- /.page-title -->
</template>

<script>
export default {
  name: 'PageTitle',
  props: ['titleInfo']

}
</script>