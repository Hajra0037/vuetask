<template>
  <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
    <v-card class="pa-0">
      <!-- <template slot="progress">
      <v-progress-linear
        color="deep-purple"
        height="10"
        indeterminate
      ></v-progress-linear>
    </template> -->
      <v-card-title>Insured Details</v-card-title>
      <v-card-text>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Type</div>
          <div class="col-5">student</div>
          <div class="col-1 pa-0 ma-0"></div>
        </v-row>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Name</div>
          <div class="col-5">Ali Ahmad</div>
          <div class="col-1 pa-0 ma-0"></div>
        </v-row>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Gender</div>
          <div class="col-5">Male</div>
          <div class="col-1 pa-0 ma-0">
            <v-icon>{{ icons.mdiPencil }}</v-icon>
          </div>
        </v-row>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Date of Birth</div>
          <div class="col-5">10 Aprial 1990</div>
          <div class="col-1 pa-0 ma-0"></div>
        </v-row>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Personal Email Address</div>
          <div class="col-5">N/A</div>
          <div class="col-1 pa-0 ma-0">
            <v-icon>{{ icons.mdiPencil }}</v-icon>
          </div>
        </v-row>

        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Mobile Phone</div>
          <div class="col-5">N/A</div>
          <div class="col-1 pa-0 ma-0">
            <v-icon>{{ icons.mdiPencil }}</v-icon>
          </div>
        </v-row>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Passport</div>
          <div class="col-5"></div>
          <div class="col-1 pa-0 ma-0">
            <v-icon>{{ icons.mdiPencil }}</v-icon>
          </div>
        </v-row>
        <v-row class="ma-0 align-center">
          <div class="text-subtitle-1 col-6">Country of residance</div>
          <div class="col-5">country</div>
          <div class="col-1 pa-0 ma-0">
            <v-icon>{{ icons.mdiPencil }}</v-icon>
          </div>
        </v-row>
      </v-card-text>
    </v-card>
    <ActivePolicyCard />
  </div>
</template>

<script>
import ActivePolicyCard from "./ActivePolicy-card.vue";
import { mdiPencil } from "@mdi/js";

export default {
  components: {
    ActivePolicyCard,
  },
  data: () => ({
    drawer: null,
    icons: {
      mdiPencil,
    },
  }),
};
</script>
