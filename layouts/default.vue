<template>
   <v-app id="inspire">
    <Appbar />
    <v-content>
      <Nuxt />
    </v-content>
  </v-app>
</template>

<script>
import Appbar from '../components/Appbar'

export default {
  components:{
    Appbar
  }
}
</script>

<style>

</style>
