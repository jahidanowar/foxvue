<template>
  <v-container fluid class="primary">
    <v-container>
      <div class="call-to-action text-center content-area">
        <h3 class="display-1 white--text mb-10 font-weight-bold">{{title}}</h3>
        <v-btn depressed large color="white" outlined tile nuxt :to="to">{{buttonText}}</v-btn>
      </div>
    </v-container>
  </v-container>
</template>

<script>
export default {
  name: "CallToAction",
  props: {
      title: String,
      buttonText: String,
      to: String
  }
}
</script>

<style>

</style>