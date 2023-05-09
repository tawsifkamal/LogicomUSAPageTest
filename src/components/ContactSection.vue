<template>
  <v-row>
    <v-col cols="6">
      <v-text-field
        label="Contact Phone"
        variant="solo"
        bg-color="blue-lighten-5"
      ></v-text-field>
    </v-col>

    <v-col cols="6">
      <v-text-field
        label="Contact Email"
        variant="solo"
        bg-color="blue-lighten-5"
      ></v-text-field>
    </v-col>
  </v-row>
</template>

<script>

export default {
  name: 'ContactSection'
}
</script>