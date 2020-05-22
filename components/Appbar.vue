<template>
    <v-container>     
    <v-app-bar
    color="bg"
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

            <div class="hidden-xs-only">
                <v-btn nuxt to="/about" text>About</v-btn>
                <v-btn nuxt to="/our-works" text>Works</v-btn>
                <v-btn nuxt to="/services" text>Service</v-btn>
                <v-btn nuxt to="/contact" text>Contact</v-btn>
            </div>
            <div class="tool">
                <v-btn icon @click="toogleMode"><v-icon>{{modeIcon}}</v-icon></v-btn>
            </div>

            <v-btn text icon color="primary" class="hidden-md-and-up" @click="drawer =! drawer">
                <v-icon>mdi-menu</v-icon>
            </v-btn>
        </v-app-bar>

        <v-navigation-drawer v-model="drawer" app temporary fixed bottom clipped>
             <v-list>
                <v-list-item
                v-for="item in items"
                :key="item.title"
                link
                :to="item.to" nuxt
                >
                <!-- <v-list-item-icon>
                    <v-icon>{{ item.icon }}</v-icon>
                </v-list-item-icon> -->

                <v-list-item-content>
                    <v-list-item-title class="text-center">{{ item.title }}</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
            </v-list>
        </v-navigation-drawer>
    </v-container>
</template>

<script>
export default {
    name: "AppBar",
    data(){
        return{
            modeIcon: "mdi-weather-night",
            drawer: false,
            items:[
                { title: 'About Us', to: '/about' },
                { title: 'Services', to: '/services' },
                { title: 'Our Works', to: '/our-works' },
                { title: 'Contact', to: '/contact' },
            ]
        }
    },
    methods: {
        toogleMode(){
            this.$vuetify.theme.dark = ! this.$vuetify.theme.dark
            this.modeIcon = this.$vuetify.theme.dark ? "mdi-weather-sunny" : "mdi-weather-night"
        }
    }
}
</script>

<style>

</style>