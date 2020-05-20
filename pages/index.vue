<template>

<<<<<<< HEAD
  <div>
  <v-container>
    <div class="header">
      <v-row align="center" justify="center">
        <v-col>
          <h1 class="header-title">We Provide Result Driven Digital Solution <span class="primary--text">.</span></h1>
          <p class="header-description">We make websites for awesome business like yours. Let us help you to make your brand online . </p>
          <v-btn color="primary" large tile depressed>Learn More</v-btn>
          <v-btn color="primary" large outlined tile class="ml-3">Let's Talk</v-btn>
        </v-col>
        <v-col align="center">
          <v-img src="https://foxflue.com/wp-content/uploads/2020/03/foxflue-web-design-illustration.png" max-width="400"></v-img>
        </v-col>
      </v-row>
    </div>
  </v-container>
  
  <v-container fluid class="primary">
    <v-container>
      <v-row>
        <v-col md="4">
          <v-card flat >
            <h2 class="countdown text-center">349 +</h2>
            <v-card-text class="text-center">businesses have thier place on Internet</v-card-text>
          </v-card>
        </v-col>
        <v-col md="4">
          <v-card flat >
            <h2 class="countdown text-center">113 +</h2>
            <v-card-text class="text-center">businesses have thier place on Internet</v-card-text>
          </v-card>
        </v-col>
        <v-col md="4">
          <v-card flat >
            <h2 class="countdown text-center">150 +</h2>
            <v-card-text class="text-center">businesses have thier place on Internet</v-card-text>
          </v-card>
        </v-col>
      </v-row>
=======
   <v-container>
     <div class="header">
       <v-row align="center" justify="center">
         <v-col>
           <h1 class="header-title">We Provide Result Driven Digital Solution<span class="primary--text">.</span></h1>
           <p class="header-description">We make websites for awesome business like yours. Let us help you to make your brand online . </p>
           <v-btn color="primary" large tile depressed>Learn More</v-btn>
           <v-btn color="primary" large outlined tile class="ml-3">Let's Talk</v-btn>
         </v-col>
         <v-col align="center">
           <v-img src="https://foxflue.com/wp-content/uploads/2020/03/foxflue-web-design-illustration.png" max-width="400"></v-img>
         </v-col>
       </v-row>
     </div>
     <div class="content-area">
       <Heading title="What We Do ?" height=5 />
       <v-row>
         <v-col cols="12" md="6" sm="12" xs="12" v-for="service in services" :key="service.title">
           <Blurb size="100" :title="service.title" :description="service.description" :image="service.image" />
         </v-col>
       </v-row>
     </div>
>>>>>>> c715dab9abf384424572e96dc28a6e398f260d9d
    </v-container>
  </v-container>

  <v-container>
    <div class="content-area">
      <div class="content-area-title text-center">
        <hr class="divider">
        <h2>What We Do ?</h2>
      </div>
    </div>
  </v-container>

  </div>
    

</template>

<script>
import Logo from '~/components/Logo.vue'
import Blurb from '~/components/Blurb.vue'
import Heading from '~/components/Heading'

export default {
  components: {
    Logo,
    Blurb,
    Heading
  },
  data(){
    return{
      title: "Foxflue Network",
      description: "We make websites for awesome business like yours. Let us help you to make your brand online.",
      services: [
        {
          image: "https://foxflue.com/wp-content/uploads/2020/03/website-design-development.png",
          title: "Web Development",
          description: "Combining detailed planning with user-centric designs, Team Foxflue deliver digital experiences that enhance conversions and engagement."
        },
        {
          image: "https://foxflue.com/wp-content/uploads/2020/03/search-engine-optimization.png",
          title: "Digital Marketing",
          description: "As a SEO, web design and development Google certified agency, we create digital marketing, SEO and paid ad (PPC) strategies that deliver industry-leading returns."
        },
        {
          image: "https://foxflue.com/wp-content/uploads/2020/03/logo-design-and-brand-design.png",
          title: "Logo Design & Branding",
          description: "Graphic designing is a very useful thing when it comes to making something more expressive. To paraphrase an old proverb ’A picture speaks a thousand words'"
        },
        {
          image: "https://foxflue.com/wp-content/uploads/2020/03/mobile-application-development.png",
          title: "Apps Development",
          description: "By blending aesthetics and functionality our Foxflue Team and iOS and Android app development team creates mobile applications that stand out in the competitive mobile space."
        },

      ]
    }
  },
  head(){
    return{
      title: this.title,
      meta: [
        {
          hid: "description",
          name: "description",
          content: this.description 
        }
      ]
    }
  }
}
</script>

<style lang="scss">
.header{
  padding: 5% 0;
  &-title{
    font-size: 3.5rem;
    margin-bottom: 1rem;
  }
  &-description{
    font-size: 1.4rem;
    margin-bottom: 1rem;
  }
}
.content-area{
  padding: 5% 0;
}
.countdown{
  text-align: center;
  font-size: 3rem;
  color: #f68c1c;
  font-weight: bold;
}
</style>
