<template>
  <v-row>
    <v-app-bar flat class="cabezera">
      <v-row class="justify-space-between lighten_grey pt-5">
        <v-col md="4">
          <v-text-field
            hide-details
            append-icon="mdi-magnify"
            filled
            placeholder="search"
            rounded
            height="20px"
            background-color="white"
          >
          </v-text-field>
        </v-col>
        <v-col md="4" class="d-flex justify-end pt-4">
          <v-badge overlap bordered color="red"  offset-x="10" offset-y="10" class="mt-3">
            <v-icon size="25px!important"> mdi-help </v-icon>
          </v-badge>
          <div class="mx-4"></div>

          <v-badge
            overlap
            bordered
            color="red"
            offset-x="10"
            offset-y="10"
            :content="messages"
            class="mt-3"
          >
            <v-icon size="25px!important"> mdi-bell </v-icon>
          </v-badge>
          <div class="mx-4"></div>
          <v-avatar size="40">
            <v-img src="https://cdn.vuetifyjs.com/images/lists/2.jpg"></v-img>
          </v-avatar>
          <div class="mr-7"></div>
        </v-col>
      </v-row>
    </v-app-bar>
  </v-row>
</template>

<script>
export default {
  name: "Cabezera",
  data() {
    return {
      messages: 0,
      show: false,
    };
  },
};
</script>

<style scoped>
.v-icon.v-icon{
  font-size: 25px!important;
}
i.v-icon.notranslate.mdi.mdi-magnify.theme--light {
    font-size: 25px!important;
}

</style>