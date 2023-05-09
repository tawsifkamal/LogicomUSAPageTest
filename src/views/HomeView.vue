<template>
  <v-container class="my-4">
    <v-row class="justify-center mb-6">
      <h1 class="text-h4 font-weight-bold">Voice Provisioning</h1>
    </v-row>

    <v-row>
      <v-col cols="12">
        <v-select
          v-model="select"
          :items="items"
          item-title="state"
          item-value="abbr"
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

    <v-row>
      <v-col cols="6">
        <v-text-field
          label="First Name"
          variant="solo"
          bg-color="blue-lighten-5"
        ></v-text-field>
      </v-col>

      <v-col cols="6">
        <v-text-field
          label="Last Name"
          variant="solo"
          bg-color="blue-lighten-5"
        ></v-text-field>
      </v-col>
    </v-row>

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

    <v-row>
      <v-col cols="4">
        <v-select
          v-model="selectCustomer"
          :items="itemsCustomer"
          item-title="state"
          item-value="abbr"
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
          item-title="state"
          item-value="abbr"
          label="Ported"
          persistent-hint
          return-object
          bg-color="blue-lighten-5"
          variant="solo-filled"
        ></v-select>
      </v-col>
    </v-row>

    <v-row dense class="mt-10">
      <v-col cols="4">
        <v-checkbox label="Bypass E911 Address Automation"></v-checkbox>
      </v-col>

      <v-col>
        <v-alert variant="outlined" type="warning" prominent border="top">
          (By checking "Bypass E911 Address Automation" you agree to manually add this phone number and address to Bandwidth)
        </v-alert>
      </v-col>
    </v-row>

    <v-row>
      <v-col cols="4">
        <v-btn color="indigo-darken-4">
          Provision
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      select: { state: "Sprout", abbr: "FL" },
      items: [
        { state: "Florida", abbr: "FL" },
        { state: "Georgia", abbr: "GA" },
        { state: "Nebraska", abbr: "NE" },
        { state: "California", abbr: "CA" },
        { state: "New York", abbr: "NY" },
      ],
      selectCustomer: { state: "", abbr: "FL" },
      itemsCustomer: [
        { state: "Florida", abbr: "FL" },
        { state: "Georgia", abbr: "GA" },
        { state: "Nebraska", abbr: "NE" },
        { state: "California", abbr: "CA" },
        { state: "New York", abbr: "NY" },
      ],
      selectPorted: { state: "", abbr: "FL" },
      itemsPorted: [
        { state: "Florida", abbr: "FL" },
        { state: "Georgia", abbr: "GA" },
        { state: "Nebraska", abbr: "NE" },
        { state: "California", abbr: "CA" },
        { state: "New York", abbr: "NY" },
      ],
    };
  },
};
</script>
