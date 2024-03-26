<script setup>

  defineProps(['item']);
</script>

<template>
  <v-card class="mt-5 h-100">

    <div class="text-center">
      <v-avatar size="150">
        <img src="" width="150" alt="Avatar">
      </v-avatar>
      <v-card-title>{{ item.title }} {{ item.subtitle }}</v-card-title>
    </div>

    <v-card-text class="">
      <div><strong>detail:</strong> {{ item.detail }}</div>
    </v-card-text>

  </v-card>
</template>
