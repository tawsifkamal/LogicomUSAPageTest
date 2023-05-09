<template>
  <v-container class="my-4">
    <!-- Title -->
    <v-row class="justify-center mb-6">
      <h1 class="text-h4 font-weight-bold">Voice Provisioning</h1>
    </v-row>

    <!-- All Text Field + Select Sections -->
    <PartnerSection />
    <NameSection />
    <AddressSection />
    <ContactSection />
    <CustomerSection />
    <E911Section />

    <!-- Provision Button -->
    <v-row>
      <v-col cols="4">
        <v-btn color="indigo-darken-4"> Provision </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import NameSection from "../components/NameSection.vue";
import AddressSection from "../components/AddressSection.vue";
import CustomerSection from "../components/CustomerSection.vue";
import ContactSection from "../components/ContactSection.vue";
import PartnerSection from "../components/PartnerSection.vue";
import E911Section from "@/components/E911Section.vue";

export default {
  components: {
    NameSection,
    ContactSection,
    AddressSection,
    CustomerSection,
    PartnerSection,
    E911Section,
  },
};
</script>
