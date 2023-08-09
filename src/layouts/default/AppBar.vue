<template>
  <div>
    <v-responsive>
      <v-img
        class="mx-auto"
        max-width="500"
        src="@/assets/SinupanSingsing.jpg"
      ></v-img>
    </v-responsive>
    <div class="mx-10">
      <v-tabs v-model="tab">
        <v-tab value="home">Aláya (Home)</v-tab>
        <v-tab value="two">Íkami (About Us)</v-tab>
        <v-tab value="three">Kagánápan (Events)</v-tab>
        <v-tab>Kasulatan (Articles)</v-tab>
      </v-tabs>
      <v-window class="" v-model="tab">
        <v-window-item value="home"> <LandingPage /> </v-window-item>

        <v-window-item value="two"> Two </v-window-item>

        <v-window-item value="three"> Three </v-window-item>
      </v-window>
    </div>
  </div>
</template>

<script setup>
import LandingPage from "@/components/LandingPage.vue";
import { ref } from "vue";
const tab = ref(null);
</script>
