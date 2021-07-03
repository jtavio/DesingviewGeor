<template>
      <v-row class="justify-space-between lighten_grey px-4 pt-10">
          <v-col sm="4" md="4" lg="4">
              <div class="info-cal">
                  <p class="font-weight-bold mb-0">Planila de pagos</p>
                  <p class="font-weight-medium mb-0">Del 01 julio al 15 de julio 2020</p>
                  <p class="text--disabled">Los calculos se estan realizando por quincenas</p>
              </div>
          </v-col>
          <v-col class="" sm="4" md="4" lg="4">
            <div class="float-right">
                <v-spacer></v-spacer>
                <v-btn
                    color="deep-purple accent-4"
                    text
                >
                    <span class="light-blue--text accent-3 text-capitalize">Invitar</span>

                    <v-icon dark color="light-blue accent-2" size="25px!important">mdi-plus-box</v-icon>
                </v-btn>
                <v-btn icon>
                    <v-icon size="25px!important">mdi-dots-vertical</v-icon>
                </v-btn>
            </div>
          </v-col>
      </v-row>

</template>

<script>
export default {
 name:'TableInfo'
}
</script>

<style>
.info-cal p{
    font-size: 14px!important;
}

</style>