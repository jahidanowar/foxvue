<template>

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
     <div class="content-area">
       <div class="content-area-title text-center">
         <hr class="divider">
         <h2>What We Do ?</h2>
       </div>
     </div>
    </v-container>

</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  data(){
    return{
      title: "Foxflue Network",
      description: "We make websites for awesome business like yours. Let us help you to make your brand online."
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
.divider{
  border: 3px solid #f68c1c;
  width: 50px;
  margin: 0 auto;
  margin-bottom: 10px;
}
.header{
  &-title{
    font-size: 3.5rem;
    margin-bottom: 1rem;
  }
  &-description{
    font-size: 1.2rem;
    margin-bottom: 1rem;
  }
}
.content-area{
  padding: 5% 0;
  &-title{
    h2{
      font-size: 2rem;
    }
  }
}
</style>
