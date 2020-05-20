<template>
    <v-card color="bg" flat min-height="280">
        <p class="pa-5">
        <slot></slot>
        </p>
        <v-card-actions>
        <v-list-item class="grow">
        <v-list-item-avatar>
            <v-img
            class="elevation-6"
            :src="avatar"
            ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
            <v-list-item-title>{{name}} <br> <span class="caption">{{designation}}</span></v-list-item-title>
        </v-list-item-content>

        </v-list-item>
        </v-card-actions>
    </v-card>
</template>

<script>
export default {
    name: "Testimonial",
    props: {
        backgroundColor: String,
        name: String,
        designation: String,
        avatar: String
    }
}
</script>

<style>

</style>