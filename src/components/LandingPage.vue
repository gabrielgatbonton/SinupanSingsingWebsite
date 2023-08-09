<template>
    <v-container>
        <v-row no-gutters>
            <v-col cols="7">
                <v-container class="px-0">
                    <v-row>
                        <v-col cols="12" class="px-0">
                            <v-card rounded="lg" flat class="bg-grey-lighten-5">
                                <v-card-text>Hello World</v-card-text>
                            </v-card>
                        </v-col>
                    </v-row>
                </v-container>
            </v-col>
        </v-row>
    </v-container>
</template>

<script setup>
import { ref } from 'vue'
const data = ref([])
</script>

<style scoped>

</style>