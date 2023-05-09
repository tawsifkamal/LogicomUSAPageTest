<template>
  <v-row>
      <v-col cols="3">
        <v-text-field
          label="Address"
          variant="solo"
          bg-color="blue-lighten-5"
        ></v-text-field>
      </v-col>

      <v-col cols="3">
        <v-text-field
          label="City"
          variant="solo"
          bg-color="blue-lighten-5"
        ></v-text-field>
      </v-col>

      <v-col cols="3">
        <v-text-field
          label="State"
          variant="solo"
          bg-color="blue-lighten-5"
        ></v-text-field>
      </v-col>

      <v-col cols="3">
        <v-text-field
          label="Zip"
          variant="solo"
          bg-color="blue-lighten-5"
        ></v-text-field>
      </v-col>
    </v-row>
</template>

<script>

export default {
  name: 'AddressSection'
}

</script>