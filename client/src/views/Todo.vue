<template>
  <div class="about">
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <div class="title">Todo</div>
      </div>

      <v-spacer></v-spacer>
      <div>
        <v-menu offset-y>
          <template v-slot:activator="{ on }">
            <v-btn v-on="on" text>
              <v-icon>mdi-account</v-icon>
              <span class="mr-2">user</span>
            </v-btn>
          </template>
          <v-list>
            <v-list-item>
              <v-list-item-title>Lorem.</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title>Lorem</v-list-item-title>
            </v-list-item>
            <v-list-item>
              <v-list-item-title>Lorem</v-list-item-title>
            </v-list-item>
          </v-list>
        </v-menu>
      </div>
    </v-app-bar>
    <v-container fluid>
      <v-row class="justify-center align-center" style="height: 80vh">
        <v-card outlined flat max-width="600" class="pa-3" dark>
          <v-text-field
            label="Task"
            outlined
            placeholder="Add to your todo list"
          ></v-text-field>
          <div class="text-center" style="margin-top: -20px">
            <v-btn color="success" v-if="!update" class="mb-3" dark
              >Submit</v-btn
            >
            <v-btn color="info" class="mb-3" v-else dark>Update</v-btn>
          </div>
          <v-divider></v-divider>
          <v-row class="align-center">
            <v-col cols="9">
              <div class="subtitle-2">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </div>
            </v-col>
            <v-col cols="3">
              <div class="d-flex justify-end">
                <v-btn color="primary" class="mr-2" small dark>edit</v-btn>
                <v-btn color="red accent-4" small dark>delete</v-btn>
              </div>
            </v-col>
            <v-col cols="12" class="py-0">
              <v-divider></v-divider>
            </v-col>
          </v-row>
          <v-row class="align-center">
            <v-col cols="9">
              <div class="subtitle-2">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </div>
            </v-col>
            <v-col cols="3">
              <div class="d-flex justify-end">
                <v-btn color="primary" class="mr-2" small dark>edit</v-btn>
                <v-btn color="red accent-4" small dark>delete</v-btn>
              </div>
            </v-col>
            <v-col cols="12" class="py-0">
              <v-divider></v-divider>
            </v-col>
          </v-row>
          <v-row class="align-center">
            <v-col cols="9">
              <div class="subtitle-2">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </div>
            </v-col>
            <v-col cols="3">
              <div class="d-flex justify-end">
                <v-btn color="primary" class="mr-2" small dark>edit</v-btn>
                <v-btn color="red accent-4" small dark>delete</v-btn>
              </div>
            </v-col>
            <v-col cols="12" class="py-0">
              <v-divider></v-divider>
            </v-col>
          </v-row>
        </v-card>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {
      update: false,
    }
  },
}
</script>
