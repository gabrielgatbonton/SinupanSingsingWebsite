<template>
  <v-container>
    <v-row no-gutters>
      <v-col cols="7">
        <v-container class="px-0">
          <v-row>
            <v-col cols="12" class="px-0">
              <v-card rounded="lg" flat class="bg-grey-lighten-3">
                <v-container>
                  <v-row no-gutters>
                    <v-col cols="auto">
                      <v-btn variant="plain">Articles</v-btn>
                      <div class="ml-3 text-h4">{{ title }}</div>
                      
                      <div class="mx-3">{{ content }}</div>
                    </v-col>
                  </v-row>
                </v-container>
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
  content: ref(
    "Kapampángans are killing Kapampángans. Not by guns nor swords, nor weapons of any kind… but by linguicide. It’s easy to observe that Kapampángan parents have consciously decided not to teach the Kapampángan language to their children. You can see it in malls, public spaces, and homes, where parents talk fluently to each other in Kapampángan, […]"
  ),
});

// You can access the variables like this:
const title = data.title;
const content = data.content;
</script>

<style scoped></style>
