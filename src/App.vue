<template>
  <v-app>
   <v-container fluid class="pa-0">
     <v-row no-gutters>
       <v-col class="light" 
        cols="2" sm="2" md="2" lg="2" xl="2">
          <!-- <PlanillaPago/>  -->
          <MenuList/> 
       </v-col>
       <v-col class="lighten_grey"
        cols="10" sm="10" md="10" lg="10" xl="10"
        >
        <div class="">
          <Cabezera/>
        </div>
        <div class="">
          <TableInfo/>
        </div>
        <div class="">
          <ModalDetalle/>
        </div>
        
          
       </v-col>
     </v-row>
   </v-container>

  </v-app>
</template>

<script>

import Cabezera from './components/Cabezera';
import TableInfo from './components/TableInfo';
import ModalDetalle from './components/ModalDetalle';
import MenuList from './components/MenuList';
export default {
  name: 'App',
 
  components: {
    MenuList,
    Cabezera,
    TableInfo,
    ModalDetalle
  },

  data: () => ({
    //
  }),
};
</script>
<style>
*{
  font-family: 'Roboto', sans-serif;
  font-size: 11px!important;
}
</style>
