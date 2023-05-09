<template>
  <v-row>
    <v-col cols="4">
      <v-select
        v-model="selectCustomer"
        :items="itemsCustomer"
        item-title="option"
        label="Customer Type"
        persistent-hint
        return-object
        bg-color="blue-lighten-5"
        class="mb-6"
        variant="solo-filled"
      ></v-select>
    </v-col>

    <v-col cols="4">
      <v-text-field
        label="Phone Number to Provision"
        variant="solo"
        bg-color="blue-lighten-5"
      ></v-text-field>
    </v-col>

    <v-col cols="4">
      <v-text-field
        label="Sip Password"
        variant="solo"
        bg-color="blue-lighten-5"
      ></v-text-field>
    </v-col>
  </v-row>

  <v-row dense>
    <v-col cols="4">
      <v-select
        v-model="selectPorted"
        :items="itemsPorted"
        item-title="option"
        label="Ported"
        persistent-hint
        return-object
        bg-color="blue-lighten-5"
        variant="solo-filled"
      ></v-select>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: "CustomerSection",
  data() {
    return {
      selectCustomer: { option: "" },
      itemsCustomer: [{ option: "Option 1" }, { option: "Option 2" }],
      selectPorted: { option: "" },
      itemsPorted: [{ option: "Option 1" }, { option: "Option 2" }],
    };
  },
};
</script>
