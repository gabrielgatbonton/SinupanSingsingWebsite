<template>
  <v-container>
    <v-row>
      <v-col cols="7">
        <v-container class="">
          <v-row>
            <v-col cols="12" class="px-0">
              <v-card rounded="lg" flat class="bg-grey-lighten-4">
                <v-container>
                  <v-row>
                    <v-col cols="auto">
                      <v-btn variant="plain">Articles</v-btn>
                      <div class="ml-3 text-h4">{{ title }}</div>
                      <div class="mx-4 text-subtitle-2 text-grey-darken-1">{{ date }}</div>

                      <div class="ma-3">{{ content }}</div>
                    </v-col>
                  </v-row>
                  <v-row class="mx-1">
                    <v-col cols="auto">
                      <v-icon size="x-large" color="info">mdi-facebook</v-icon>
                    </v-col>
                    <v-spacer></v-spacer>
                    <v-col cols="auto">
                      <v-icon size="x-large" color="grey-darken-2"
                        >mdi-arrow-bottom-right</v-icon
                      >
                    </v-col>
                  </v-row>
                </v-container>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-col>
      <v-col cols="5">
        <v-container>
          <v-row>
            <v-col cols="12">
              <v-card rounded="lg" flat>
                <div class="text-h6 font-weight-bold">Recent Posts</div>
                <v-divider color="#000000" class="border-opacity-100" :thickness="3"></v-divider>
                <div class="my-3">
                  <v-card flat>
                    <div class="text-">Some text here</div>
                  </v-card>
                </div>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-col>
    </v-row>
  </v-container>
</template>

<script setup>
import { reactive, ref } from "vue";
// Create a reactive object using the reactive function
const data = reactive({
  title: ref("Kapampángan Language is “Definitely Endangered” - UNESCO"),
  date: ref("March 7, 2019"),
  content: ref(
    "Kapampángans are killing Kapampángans. Not by guns nor swords, nor weapons of any kind… but by linguicide. It’s easy to observe that Kapampángan parents have consciously decided not to teach the Kapampángan language to their children. You can see it in malls, public spaces, and homes, where parents talk fluently to each other in Kapampángan, […]"
  ),
});

// You can access the variables like this:
const title = data.title;
const content = data.content;
const date = data.date;
</script>

<style scoped></style>
