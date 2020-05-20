<template>
  <div class="our-works">
    <PageHero title="Our Works">Website Design is Not only Our Profession, It’s Our Passion</PageHero>
  </div>
</template>

<script>
import PageHero from "~/components/PageHero"
export default {
    data(){
        return{
            title: "Our Works",
            description: "About Us Meta Descrituion"
        }
    },
    components: {
        PageHero
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