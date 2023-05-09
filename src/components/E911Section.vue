<template>
  <v-row dense class="mt-10">
      <v-col cols="4">
        <v-checkbox label="Bypass E911 Address Automation"></v-checkbox>
      </v-col>

      <v-col>
        <v-alert variant="outlined" type="warning" prominent border="top">
          (By checking "Bypass E911 Address Automation" you agree to manually
          add this phone number and address to Bandwidth)
        </v-alert>
      </v-col>
    </v-row>
</template>

<script>
export default {
  name: 'E911Section'
}
</script>