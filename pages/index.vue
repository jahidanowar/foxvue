<template>

   <v-container>
     <div class="header">
       <v-row align="center" justify="center">
         <v-col>
           <h1 class="header-title">Hellow World</h1>
           <p class="header-description">We make websites for awesome business like yours. Let us help you to make your brand online.</p>
           <v-btn color="success">Learn More</v-btn>
           <v-btn color="success">Let's Talk</v-btn>
         </v-col>
         <v-col align="center">
           <v-img src="https://foxflue.com/wp-content/uploads/2020/03/foxflue-web-design-illustration.png" max-width="400"></v-img>
         </v-col>
       </v-row>
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
.header{
  &-title{
    font-size: 3.5rem;
    text-transform: uppercase;
  }
  &-description{

  }
}
</style>
