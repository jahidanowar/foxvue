<template>
    <v-card color="#fafafa" flat>
        <p class="pa-5 font-weight-bold">
        "<slot></slot>"
        </p>
        <v-card-actions>
        <v-list-item class="grow">
        <v-list-item-avatar color="grey darken-3">
            <v-img
            class="elevation-6"
            :src="avatar"
            ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
            <v-list-item-title>{{name}}, {{designation}}</v-list-item-title>
        </v-list-item-content>

        </v-list-item>
        </v-card-actions>
    </v-card>
</template>

<script>
export default {
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