<template>
  <div>
     <v-row>

      <v-col cols="12" md="3">
     <v-card height="60" color="white">
      <v-card-text>
        <v-row>
          <v-col>
            <div class="text-center">
              <v-progress-circular :model-value="20" :rotate="360" :size="35" :width="10" color="blue">
                <template v-slot:default> {{ 20 }}%</template>
              </v-progress-circular>
            </div>
          </v-col>
          <v-col>
            <v-row no-gutters>
              <v-col cols="12" class="text-right text-uppercase">student</v-col>
              <v-col cols="12" class="text-right font-weight-bold">10</v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-card-text>
     </v-card>
      </v-col>
      <v-col cols="12" md="3">
      <v-card height="60" color="white">
      <v-card-text>

      </v-card-text>
        <v-row>
          <v-col>
            <div class="text-center">
              <v-progress-circular :model-value="20" :rotate="360" :size="35" :width="10" color="blue">
                <template v-slot:default> {{ 20 }}%</template>
              </v-progress-circular>
            </div>
          </v-col>
          <v-col>
            <v-row no-gutters>
              <v-col cols="12" class="text-right text-uppercase">student</v-col>
              <v-col cols="12" class="text-right font-weight-bold">10</v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-card>
      </v-col>
      <v-col cols="12" md="3"></v-col>
      <v-card height="60" color="white">
      </v-card>
     </v-row>

  </div>
</template>

<script lang="ts" setup>
import { v } from 'vue-router/dist/router-CWoNjPRp.mjs';

</script>

<style>
</style>