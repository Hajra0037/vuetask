<template>
  <v-card class="mx-auto pa-0 my-6">
    <v-tabs v-model="tab" align-with-title>
      <v-tabs-slider color="info"></v-tabs-slider>
      <v-tab v-for="item in items" :key="item">
        {{ item }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in items" :key="item">
        <v-card-title
          >Policy 122211
          <v-chip class="mx-2" outlined color="success">Active</v-chip>
        </v-card-title>

        <v-card-text>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Country</div>
            <div class="col-5">Country</div>
            <div class="col-1 pa-0 my-0">
              <!-- <v-icon>{{ icons.mdiPencil }}</v-icon> -->
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Issue Date</div>
            <div class="col-5">2nd sep 2022</div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Policy start Date</div>
            <div class="col-5">2nd sep 2022</div>
            <div class="col-1 pa-0 my-0">
              <!-- <v-icon>{{ icons.mdiPencil }}</v-icon> -->
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Trip start Date</div>
            <div class="col-5">2nd sep 2022</div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Trip end Date</div>
            <div class="col-5">2nd sep 2022</div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Group Name</div>
            <div class="col-5">N/A</div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Name of school</div>
            <div class="col-5">School name</div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>

          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Student</div>
            <div class="col-5">N/A</div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Address</div>
            <div class="col-5"></div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Coverage Plan</div>
            <div class="col-5"></div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
          <v-row class="my-0 align-center">
            <div class="text-subtitle-1 col-6">Country of residance</div>
            <div class="col-5"></div>
            <div class="col-1 pa-0 my-0">
              <v-icon>{{ icons.mdiPencil }}</v-icon>
            </div>
          </v-row>
        </v-card-text>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
import { mdiPencil } from "@mdi/js";

export default {
  data() {
    return {
      tab: null,
      items: ["Active Policy", "Previous Policy"],
      icons: {
        mdiPencil,
      },
    };
  },
};
</script>
