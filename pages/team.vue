<template>
  <div>
     <Header :logo_url="logo_url" :logo_dark_url="logo_dark_url" />
    <PageTitle :titleInfo="titleInfo" />
    <div class="container">
       <h2 class="heading__title text-center mt-4">Meet Our Team</h2>
    </div>
   
    <Team :teams="teams" />
  </div>
</template>

<script>
import Header from '@/components/Header'
import PageTitle from '@/components/PageTitle'
import Team from '@/components/Team'
export default {
  head() {
    return {
      title: 'Our Team',
      script: [{ src: '/js/main.js', difer: false, ssr: true }]
    }
  },
  components: {
    Header,
    PageTitle,
    Team
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
    teams: [
      {
        id: 1,
        image: '/images/team/1.jpg',
        facebook: '#',
        twitter: '#',
        instagram: '#',
        name: 'Mike Dooley',
        designation: 'Chief Executive'
      },
      {
        id: 2,
        image: '/images/team/2.jpg',
        facebook: '#',
        twitter: '#',
        instagram: '#',
        name: 'Mr. Bhupender Singh',
        designation: 'Chief Electrical Engineer'
      },
      {
        id: 3,
        image: '/images/team/3.jpg',
        facebook: '#',
        twitter: '#',
        instagram: '#',
        name: 'Mike Dooley',
        designation: 'Marketing Executive'
      },
      {
        id: 4,
        image: '/images/team/4.jpg',
        facebook: '#',
        twitter: '#',
        instagram: '#',
        name: 'Mike Dooley',
        designation: 'Engineer'
      }
    ]
  })
}
</script>