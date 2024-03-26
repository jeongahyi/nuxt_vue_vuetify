<script setup>

const items = [{id: 1, title: "kirby", subtitle: "star", detail: "cute fighter"}];
const dataExists = items.length > 0;

</script>

<template>
  <v-container class="lighten-5 mb-6">
    <v-row align="center" justify="center" class="h-screen" v-if="!dataExists">
      <v-col cols="12" sm="8" md="6" class="text-center">
        <div class="display-1">no item found</div>
      </v-col>
    </v-row>
    <v-row>
      <v-col
          v-for="item in items"
          :key="item.id"
          cols="12"
          sm="4"
      >
        <CardItem :item="item"/>
      </v-col>
    </v-row>
    <v-row justify="center">
      <Dialog>
      </Dialog>
    </v-row>
  </v-container>
</template>