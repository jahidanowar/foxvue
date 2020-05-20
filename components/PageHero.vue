<template>
    <v-container fluid class="bg1">
        <v-container>
            <v-row align="center" justify="center">
                <v-col cols="12">
                    <h1 class="text-center">{{title}}</h1>
                    
                    <p class="text-center"><slot></slot></p>
                </v-col>
            </v-row>
        </v-container>
    </v-container>
</template>

<script>
export default {
    name: "PageHero",
    props: {
        title: String
    }
}
</script>

<style>

</style>