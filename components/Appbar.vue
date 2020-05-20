<template>
    <v-container>     
    <v-app-bar
    color="white"
    flat
        >
        
            <nuxt-link to="/">
            <v-toolbar-title>
                <v-img 
                src="https://foxflue.com/wp-content/uploads/2020/03/foxflue-logo.png"
                width="150"
                    >  
                </v-img>
            </v-toolbar-title>
            </nuxt-link>

            <v-spacer></v-spacer>

            <v-toolbar-items>
                <v-btn nuxt to="/about" text>About</v-btn>
                <v-btn nuxt to="/our-works" text>Works</v-btn>
                <v-btn nuxt to="/services" text>Service</v-btn>
                <v-btn nuxt to="/contact" text>Contact</v-btn>
            </v-toolbar-items>

        </v-app-bar>
    </v-container>
</template>

<script>
export default {
    data(){
        return{
            drawer: false
        }
    }
}
</script>

<style>

</style>