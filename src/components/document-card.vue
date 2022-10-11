<template>
  <div class="col-lg-6 col-md-6 col-sm-12 col-xs-12">
    <v-card class="mx-auto pa-0">
      <template slot="progress">
        <v-progress-linear
          color="deep-purple"
          height="10"
          indeterminate
        ></v-progress-linear>
      </template>

      <v-card-title>Document Details</v-card-title>

      <v-card-text>
        <v-row class="ma-0 align-center">
          <v-checkbox
            v-model="ex4"
            label="Visa Letter"
            color="info"
            value="Visa Letter"
            hide-details
          ></v-checkbox>
          <!-- <div class="col-1 pa-0 ma-0">edit</div> -->
        </v-row>
        <v-row class="ma-0 align-center">
          <v-checkbox
            v-model="ex4"
            label="Document Name"
            color="info"
            value="Visa Letter"
            hide-details
          ></v-checkbox>
          <!-- <div class="col-1 pa-0 ma-0">edit</div> -->
        </v-row>
        <v-row class="ma-0 align-center">
          <v-checkbox
            label="Document Name"
            color="info"
            value="Visa Letter"
            hide-details
          ></v-checkbox>
          <!-- <div class="col-1 pa-0 ma-0">edit</div> -->
        </v-row>
      </v-card-text>
    </v-card>
    <v-card class="mx-auto pa-0 my-6">
      <template slot="progress">
        <v-progress-linear
          color="deep-purple"
          height="10"
          indeterminate
        ></v-progress-linear>
      </template>

      <v-card-title>Change History</v-card-title>

      <!-- <v-card-text> -->
      <v-stepper vertical>
        <v-stepper-step :complete="e6 > 1" step="1">
          Select an app
          <small>Summarize if needed</small>
        </v-stepper-step>

        <v-stepper-step :complete="e6 > 2" step="2">
          Select an ad format and name ad unit
          <small>Summarize if needed</small>
        </v-stepper-step>
      </v-stepper>

      <!-- </v-card-text> -->
    </v-card>
  </div>
</template>
