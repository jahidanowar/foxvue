<template>
<div>
  <!-- Hero Area Starts -->
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
  </v-container>
  <!-- Hero Area Ends -->

  <!-- Counter -->
  <v-container fluid class="primary">
    <v-container>
      <v-row>
        <v-col md="4" sm="12" cols="12" xs="12">
          <v-card flat >
            <h2 class="countdown text-center">349 +</h2>
            <v-card-text class="text-center">businesses now have thier place on Internet</v-card-text>
          </v-card>
        </v-col>
        <v-col md="4" sm="12" cols="12" xs="12">
          <v-card flat >
            <h2 class="countdown text-center">113 +</h2>
            <v-card-text class="text-center">businesses now have their identity</v-card-text>
          </v-card>
        </v-col>
        <v-col md="4" sm="12" cols="12" xs="12">
          <v-card flat >
            <h2 class="countdown text-center">150 +</h2>
            <v-card-text class="text-center">happy clients</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
  <!-- Counter Ends  -->

  <!-- Service Area  -->
  <v-container>
    <div class="content-area">
       <Heading title="What We Do ?" :height="5" />
       <v-row>
         <v-col cols="12" md="6" sm="12" xs="12" v-for="service in services" :key="service.title">
           <Blurb size="100" :title="service.title" :description="service.description" :image="service.image" />
         </v-col>
       </v-row>
     </div>
  </v-container>
  <!-- Service Area Ends  -->

  <!-- Testimonials  -->
  <v-container>
    <div class="content-area">
       <Heading title="What Clients Say About Us" :height="5" />
       <v-row>
         <v-col cols="12" md="4" sm="6" v-for="testimonial in testimonials" :key="testimonial.name">
           <Testimonial 
           :name="testimonial.name" 
           :avatar="testimonial.avatar"
           :designation="testimonial.designation" 
           > 
           "{{testimonial.review}}"
           </Testimonial>
         </v-col>
       </v-row>
     </div>
  </v-container>
  <!-- Testimonials Ends  -->

  <!-- Call to action -->
  <v-container fluid class="primary">
    <v-container>
      <div class="call-to-action text-center content-area">
        <h3 class="display-1 white--text mb-10 font-weight-bold">Ready to Create The Next Big Thing?</h3>
        <v-btn depressed large color="white" outlined tile nuxt to="/contact">Let's Start a Project</v-btn>
      </div>
    </v-container>
  </v-container>
  <!-- Call to action Ends -->


  </div>
</template>

<script>
import Blurb from '~/components/Blurb.vue'
import Heading from '~/components/Heading'
import Testimonial from '~/components/Testimonial'

export default {
  components: {
    Blurb,
    Heading,
    Testimonial
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

      ],
      testimonials: [
        {
          name: "Jaideep Hinduja",
          designation: "Director, SimexT",
          avatar: "https://jahid.dev/wp-content/uploads/2020/04/hasan-alkhater.jpg",
          review: "They understands the requirements quite well, and implementation is praiseworthy. They puts in their minds and gives real good practical suggestions. Would surely work on more projects with Foxflue in future.",
        },
        {
          name: "Thomas Chris",
          designation: "Owner, BrosMobileParts",
          avatar: "https://jahid.dev/wp-content/uploads/2020/04/hasan-alkhater.jpg",
          review: "I really like working with Foxflue. They have a lot of experience with WordPress, are friendly and doesn’t stop working until you are completely satisfied with the result. 5 well-deserved stars",
        },
        {
          name: "Dulen Scevnder",
          designation: "Director, BanomeKoffie",
          avatar: "https://jahid.dev/wp-content/uploads/2020/04/hasan-alkhater.jpg",
          review: "Jahid took time to understand the requirements and finished before the deadline set. His task was to create a multi-lingual landing page with automatic language change based on location, and he did it successfully in a timely manne",
        }
      ],
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
