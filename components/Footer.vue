<template>
<div>
  <footer id="footer" class="footer footer-1">
      <div class="footer-top">
        <div class="container">
          <div class="row">
            <div class="col-sm-12 col-md-12 col-lg-4 footer__widget footer__widget-about  mb-30">
              <div class="footer__widget-content">
                <img src="/images/logo/logo_square.svg" width="50%" alt="logo">
                <p>Unit 23, Xokyai Village, Xaysettha District,<br>Vientiane Capital, Lao P.D.R.</p>
                <p>Mail: <a href="mailto:dokkhoundolecoltd@gmail.com">dokkhoundolecoltd@gmail.com</a></p>
              </div>
            </div><!-- /.col-lg-4 -->
            <div class="col-6 col-sm-6 col-md-3 col-lg-2 footer__widget footer__widget-nav">
              <h6 class="footer__widget-title">Company</h6>
              <div class="footer__widget-content">
                <nav>
                  <ul class="list-unstyled">
                    <li><nuxt-link to="/about">About Us</nuxt-link></li>
                    <li><nuxt-link to="/team">Meet Our Team</nuxt-link></li>
                    <li><nuxt-link to="/portfolio">Portfolio</nuxt-link></li>
                    <li><nuxt-link to="/products">Products</nuxt-link></li>
                    <li><nuxt-link to="/contact">Contacts</nuxt-link></li>
                  </ul>
                </nav>
              </div><!-- /.footer-widget-content -->
            </div><!-- /.col-lg-2 -->
            <div class="col-6 col-sm-6 col-md-3 col-lg-2 footer__widget footer__widget-nav">
              <h6 class="footer__widget-title">References</h6>
              <div class="footer__widget-content">
                <nav>
                  <ul class="list-unstyled">
                    <li><a href="#">Lao Ford City</a></li>
                    <li><a href="#">Nova Lao Sole., Ltd</a></li>
                    <li><a href="#">Leusay Saysana Sole Co.,Ltd</a></li>
                    <li><a href="#">Busan national university</a></li>
                    <li><a href="#">Yang-Ju city Hall </a></li>
                    <li><a href="#">Korea military academy</a></li>
                  </ul>
                </nav>
              </div><!-- /.footer-widget-content -->
            </div><!-- /.col-lg-2 -->
            <div class="col-12 col-sm-12 col-md-6 col-lg-4 footer__widget">
              <div class="footer__widget-content">
                <h6 class="footer__widget-title">Contact on Phone</h6>
                <p>Please feel to contact us anytime with the following numbers</p>
                <p><a href="tel:+856 20 2222 3410" class="font-weight-bold color-white">(856) 20 2222 3410</a></p>
                <p><a href="tel:+856 20 5492 1515" class="font-weight-bold color-white">(856) 20 5492 1515 </a></p>
                <p><a href="tel:+856 20 5457-7181" class="font-weight-bold color-white">(856) 20 5457-7181</a></p>
                <p><a href="tel:+856 20 5569 6262" class="font-weight-bold color-white">(856) 20 5569 6262</a></p>
                <!-- <form class="widget__newsletter-form">
                  <div class="form-group mb-0">
                    <input type="text" class="form-control" placeholder="Your Email Address ">
                    <button type="submit" class="btn btn__primary btn__hover2">Subscribe</button>
                  </div>
                </form> -->
              </div><!-- /.footer-widget-content -->
            </div><!-- /.col-lg-4 -->
          </div><!-- /.row -->
        </div><!-- /.container -->
      </div><!-- /.footer-top -->
      <div class="footer-bottom">
        <div class="container">
          <div class="row">
            <div class="col-sm-12 col-md-9 col-lg-9">
              <div class="footer__copyright">
                <nav>
                  <ul class="list-unstyled footer__copyright-links d-flex flex-wrap">
                    <li>
                      <a href="http://themeforest.net/user/7oroof">
                        &copy; 2020 Dokkoun Electric Sole Co., Ltd, Powered by <span class="color-theme">Altus</span>
                      </a>
                    </li>
                    <li><a href="#">Terms & Conditions </a></li>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Sitemap</a></li>
                  </ul>
                </nav>

              </div><!-- /.Footer-copyright -->
            </div><!-- /.col-lg-6 -->
            <div class="col-sm-12 col-md-3 col-lg-3 d-flex align-items-center">
              <div class="social__icons justify-content-end w-100">
                <a href="#"><i class="fa fa-facebook"></i></a>
                <a href="#"><i class="fa fa-twitter"></i></a>
                <a href="#"><i class="fa fa-instagram"></i></a>
              </div><!-- /.social-icons -->
            </div><!-- /.col-lg-6 -->
          </div><!-- /.row -->
        </div><!-- /.Footer-bottom -->
      </div><!-- /.container -->
    </footer><!-- /.Footer -->
    <button id="scrollTopBtn" v-scroll-to="'#header'"><i class="fa fa-long-arrow-up"></i></button>
    </div>
</template>