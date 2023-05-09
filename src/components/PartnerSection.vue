<template>
  <v-row>
    <v-col cols="12">
      <v-select
        v-model="selectPartner"
        :items="itemsPartner"
        item-title="option"
        label="Select a partner"
        persistent-hint
        return-object
        bg-color="blue-lighten-5"
        class="mb-6"
        variant="solo-filled"
      ></v-select>

      <v-text-field
        label="Account Number"
        variant="solo"
        bg-color="blue-lighten-5"
      ></v-text-field>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "PartnerSection",
  data() {
    return {
      selectPartner: { option: "Sprout" },
      itemsPartner: [{ option: "Option 1" }, { option: "Option 2" }],
    };
  },
};
</script>
