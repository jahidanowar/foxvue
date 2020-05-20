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
    data(){
        return{
            drawer: false,
            items:[
                { title: 'About Us', icon: 'gavel' },
                { title: 'Services', icon: 'dashboard' },
                { title: 'Our Works', icon: 'account_box' },
                { title: 'Contact', icon: 'gavel' },
            ]
        }
    }
}
</script>

<style>

</style>