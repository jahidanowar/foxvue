<template>
  <div class="page-footer">
      <v-container fluid color="#fafafa">
          <v-container>
              <v-row align="center" justify="center">
                  <v-col cols="12" md="4" sm="12" xs=12>
                      <v-img src="https://foxflue.com/wp-content/uploads/2020/03/foxflue-network-new-logo.png" max-width="250"></v-img>
                  </v-col>
                  <v-col cols="12" md="4" sm="12" xs=12>
                     <h3>Web Design</h3>
                     <ul class="footer-menu">
                         <li>
                            <nuxt-link to="/about" class="textcolor--text">WordPress Webite Development</nuxt-link>
                         </li>
                         <li>
                            <nuxt-link to="/contact" class="textcolor--text">eCommerce Website Development</nuxt-link>
                         </li>
                         <li>
                            <nuxt-link to="/privacy-policy" class="textcolor--text">Business Website</nuxt-link>
                         </li>
                         <li>
                            <nuxt-link to="/terms-and-conditions" class="textcolor--text">Graphics Design</nuxt-link>
                         </li>
                     </ul>
                  </v-col>
                  <v-col cols="12" md="4" sm="12" xs=12>
                     <h3>Company</h3>
                     <ul class="footer-menu">
                         <li>
                            <nuxt-link to="/about" class="textcolor--text">About Us</nuxt-link>
                         </li>
                         <li>
                            <nuxt-link to="/contact" class="textcolor--text">Contact Us</nuxt-link>
                         </li>
                         <li>
                            <nuxt-link to="/privacy-policy" class="textcolor--text">Privacy Policy</nuxt-link>
                         </li>
                         <li>
                            <nuxt-link to="/terms-and-conditions" class="textcolor--text">Terms and Conditions</nuxt-link>
                         </li>
                     </ul>
                  </v-col>
              </v-row>
          </v-container>
      </v-container>
      <v-footer>
        <v-col class="text-center" cols="12">
            &copy; 2017 - {{new Date().getFullYear()}} All Rights Reseved. <nuxt-link to="/">Foxflue Network</nuxt-link> <br>
            A Private Limited Company
        </v-col>
        
      </v-footer>
  </div>
</template>

<script>
export default {
    name: "PageFooter",
}
</script>

<style lang="scss">
ul{
    margin-top:15PX;
    list-style-type: none!important;
    list-style-position: inside;
    padding-left: 0.5px!important;
    li{
        margin-bottom: 10px;
        a:link{
            text-decoration: none;
        }
       
    }
}
</style>