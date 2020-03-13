<template>
  <header id="header" class="header header-transparent">
      <nav class="navbar navbar-expand-lg sticky-navbar">
        <div class="container">
          <a class="navbar-brand" href="/">
            <img :src="logo_url" class="logo-light" alt="logo" width="50%">
            <img :src="logo_dark_url" class="logo-dark" alt="logo" width="50%">
          </a>
          <button class="navbar-toggler" type="button">
            <span class="menu-lines"><span></span></span>
          </button>
          <div class="collapse navbar-collapse" id="mainNavigation">
            <ul class="navbar-nav ml-auto">
              <li class="nav__item">
                <a href="/" class="nav__item-link active">Home</a>
              </li>
              <li class="nav__item with-dropdown">
                <a href="/about" class="dropdown-toggle nav__item-link">Company</a>
                <i class="fa fa-angle-right" data-toggle="dropdown"></i>
                <ul class="dropdown-menu">
                  <li class="nav__item"><a href="/about" class="nav__item-link">About Us</a></li>
                  <li class="nav__item"><a href="/team" class="nav__item-link">Leadership Team</a></li>
                </ul>
              </li>
              <li class="nav__item">
                <a href="/services" class="nav__item-link">Services</a>
              </li>
              <li class="nav__item">
                <a href="/products" class="nav__item-link">Products</a>
              </li>
               <li class="nav__item">
                <a href="/portfolio" class="nav__item-link">Portfolio</a>
              </li>
              <li class="nav__item">
                <a href="/contact" class="nav__item-link">Contacts</a>
              </li>
            </ul>
          </div>
          <div class="navbar-modules">
            <ul class="list-unstyled d-flex align-items-center modules__btns-list">
              <li><a href="#" class="module__btn module__btn-search"><i class="fa fa-search"></i></a></li>
              <li class="d-none d-lg-block"><a href="request-quote.html" class="btn btn__primary module__btn-request">
                  <span>Request A Quote</span><i class="icon-arrow-right2"></i>
                </a></li>
              <li class="d-none d-lg-block">
                <div class="module__btn module__btn-phone d-flex align-items-center">
                  <i class="icon-phone mr-3"></i>
                  <div>
                    <span class="d-block">Call Us:</span>
                    <a href="tel:55-654-541-17">+55 654 541 17</a>
                  </div>
                </div>
              </li>
            </ul>
          </div>
        </div>
      </nav>
    </header>
</template>

<script>
export default {
  props: ['logo_url', 'logo_dark_url']
}
</script>