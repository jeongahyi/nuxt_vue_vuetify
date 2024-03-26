<script setup>


const openModal = () => {
  console.log('open modal')
}

</script>

<template>
    <v-row justify="center">
      <v-col cols="12">
        <v-banner color="info" dark>
          <v-container>

            <v-row justify="center">
              <v-col cols="12">
                <div class="text-center">

                  <h1 class="text-blue-darken-3 mb-3 text-h4 text-sm-h3 font-weight-bold">list</h1>
                  <p class="text-sm-body-1 mb-5">to do list</p>

                  <div>
                    <v-btn color="primary" @click="openModal">Add new item</v-btn>
                  </div>

                </div>
              </v-col>
            </v-row>
          </v-container>
        </v-banner>
      </v-col>
    </v-row>
</template>