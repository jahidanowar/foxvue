<template>
  <v-container>
      About Page
  </v-container>
</template>

<script>
export default {
    data(){
        return{
            title: "About Us",
            description: "About Us Meta Descrituion"
        }
    },
    head(){
        return {
            title: this.title,
            meta:[
                {
                    hid: 'description',
                    name: 'description',
                    content: this.description
                }
            ]
        }
    }
}
</script>

<style>

</style>