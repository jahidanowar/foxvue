<template>
  <div class="services">
    <PageHero title="We help Small Business to Grow Online.">At Foxflue Network we strive to make your buisness standout and be unrivalled. <br>We have a group of highly skilled experts aiming to provide innovation and flexibility to your Business.</PageHero>
    
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


    <!-- Call to action -->
    <CallToAction title="Ready to Create The Next Big Thing?" buttonText="Start A Project" to="/contact" />
    <!-- Call to action Ends -->
  </div>
</template>

<script>
import PageHero from "~/components/PageHero"
import CallToAction from "~/components/CallToAction"
import Blurb from "~/components/Blurb"
import Heading from "~/components/Heading"

export default {
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
    components:{
        PageHero,
        CallToAction,
        Blurb,
        Heading
    }
}
</script>

<style>

</style>