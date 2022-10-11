<template>
  <v-app id="inspire">
    <v-app-bar app class="col-12 pa-0">
      <v-app-bar-nav-icon class="col-1 pa-0" @click="drawer = !drawer">
      </v-app-bar-nav-icon>
      <div class="d-flex justify-space-between align-center col-11 pa-0">
        <v-toolbar-title>Application</v-toolbar-title>
        <v-avatar color="info" size="56">HA</v-avatar>
      </div>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" fixed temporary>
      <!--  -->
    </v-navigation-drawer>

    <v-main>
      <v-container>
        <v-row class="align-center justify-center">
          <div
            class="col-xs-12 col-sm-12 col-md-6 col-lg-6 text-sm-center text-md-left text-lg-left"
          >
            <p class="ma-0">App View/Edit</p>
            <p class="font-weight-black font-size-20">James Bond</p>
          </div>
          <div
            class="d-flex justify-lg-end justify-md-center justify-sm-center justify-xs-center flex-wrap col-xs-12 col-sm-12 col-md-6 col-lg-6"
          >
            <v-btn
              class="mx-2 my-xs-1"
              outlined
              color="error"
              dark
              v-bind="attrs"
              v-on="on"
            >
              Print Insurance Card
            </v-btn>
            <v-btn
              class="my-xs-1"
              outlined
              color="info"
              dark
              v-bind="attrs"
              v-on="on"
            >
              Cancel coverage
            </v-btn>
          </div>
        </v-row>
        <v-row class="justify-center align-baseline">
          <InsureCard />
          <DocumentCard />
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import InsureCard from "./Insure-card.vue";
import DocumentCard from "./document-card.vue";

export default {
  components: {
    InsureCard,
    DocumentCard,
  },
  data: () => ({ drawer: null }),
};
</script>
