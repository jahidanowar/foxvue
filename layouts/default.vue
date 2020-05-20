<template>
   <v-app id="inspire">
    <Appbar />
    <v-content>
      <Nuxt />
    </v-content>
    <PageFooter />
  </v-app>
</template>

<script>
import Appbar from '~/components/Appbar'
import PageFooter from '~/components/PageFooter'

export default {
  components:{
    Appbar,
    PageFooter,
  }
}
</script>

<style>

@font-face {
    font-family: 'Cera Pro';
    src: url('../assets/fonts/CeraPro-Regular.eot');
    src: local('Cera Pro Regular'), local('CeraPro-Regular'),
        url('../assets/fonts/CeraPro-Regular.eot?#iefix') format('embedded-opentype'),
        url('../assets/fonts/CeraPro-Regular.woff') format('woff'),
        url('../assets/fonts/CeraPro-Regular.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
}
@font-face {
    font-family: 'Cera Pro';
    src: url('../assets/fonts/CeraPro-Light.eot');
    src: local('Cera Pro Light'), local('CeraPro-Light'),
        url('../assets/fonts/CeraPro-Light.eot?#iefix') format('embedded-opentype'),
        url('../assets/fonts/CeraPro-Light.woff') format('woff'),
        url('../assets/fonts/CeraPro-Light.ttf') format('truetype');
    font-weight: 300;
    font-style: normal;
}
@font-face {
    font-family: 'Cera Pro';
    src: url('../assets/fonts/CeraPro-Bold.eot');
    src: local('Cera Pro Bold'), local('CeraPro-Bold'),
        url('../assets/fonts/CeraPro-Bold.eot?#iefix') format('embedded-opentype'),
        url('../assets/fonts/CeraPro-Bold.woff') format('woff'),
        url('../assets/fonts/CeraPro-Bold.ttf') format('truetype');
    font-weight: bold;
    font-style: normal;
}

</style>
