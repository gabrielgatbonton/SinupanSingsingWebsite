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
                                        <div class="ml-3 text-h4">{{ value1 }}</div>
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
import { reactive, ref } from 'vue';
// Create a reactive object using the reactive function
const data = reactive({
  title: ref("Kapampángan Language is “Definitely Endangered” - UNESCO"),
  // ... other variables
});

// You can access the variables like this:
const value1 = data.title;


</script>

<style scoped>

</style>