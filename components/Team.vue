<template>
  <section id="team" class="team  text-center pt-120 pb-50">
      <div class="container">
        <div class="row">
          <!-- Member #1 -->
          <div class="col-sm-6 col-md-4 col-lg-4" v-for="(team,index) in teams" :key="index">
            <div class="member">
              <div class="member__img">
                <img :src="team.image" alt="member img">
                <div class="member__hover">
                  <div class="member__content-inner">
                    <div class="social__icons justify-content-center">
                      <a :href="team.facebook"><i class="fa fa-facebook"></i></a>
                      <a :href="team.twitter"><i class="fa fa-twitter"></i></a>
                      <a :href="team.isntagram"><i class="fa fa-instagram"></i></a>
                    </div><!-- /.social-icons -->
                  </div><!-- /.member-content-inner -->
                </div><!-- /.member-hover -->
              </div><!-- /.member-img -->
              <div class="member__info">
                <h5 class="member__name">{{team.name}}</h5>
                <p class="member__desc">{{team.designation}}</p>
              </div><!-- /.member-info -->
            </div><!-- /.member -->
          </div><!-- /.col-lg-4 -->
        </div> <!-- /.row -->
      </div><!-- /.container -->
    </section><!-- /.team5 end  -->
</template>

<script>
export default {
  props: ['teams']
}
</script>