<template>
  <div>
       <v-row class="text-center light">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-5"
          contain
          height="60"
        />     
    </v-row>
    <v-row>
        <v-col>
            <v-list class="mx-2 mt-10" flat>
                <v-list-item>
                    <v-list-item-icon>
                        <v-icon size="25px!important">mdi-view-dashboard</v-icon>
                    </v-list-item-icon>

                    <v-list-item-title  style="font-size:14px!important;">Dashboard</v-list-item-title>
                </v-list-item>
                <v-list-group  v-for="item in items"
                    :key="item.title"
                    :value="true"
                    no-action
                    v-model="item.active"
                >
                <template v-slot:activator>
                    <v-list-item-icon style="margin-right: 15px;">
                        <v-icon size="25px!important" v-text="item.action"></v-icon>
                    </v-list-item-icon>
                    <v-list-item-content>
                        <v-list-item-title style="font-size:14px!important;" v-text="item.title"></v-list-item-title>
                    </v-list-item-content>
                </template>
                <v-list-item-group
                    v-model="selectedItem"
                    sub-group
                    class="d-flex align-end flex-column" style="border-left: 1px solid rgb(0, 0, 0, 0.15);
                        width: 180px;
                        margin: 0 auto;"
                    >
                    <div  class="marcado"></div>
                    <v-list-item
                        v-for="child in item.items"
                        :key="child.title"
                        
                    >
                   <v-list-item-content>
                       
                        <v-list-item-title style="font-size:12px!important; padding:0px!important" color="red" v-text="child.title"></v-list-item-title>
                    </v-list-item-content>                      
                    </v-list-item>
                </v-list-item-group>
                </v-list-group>
            </v-list>
        </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
    MenuList:'MenuList',
    data: () => ({
        selectedItem: 1,
items: [
            {
                action : 'mdi-point-of-sale',
                items:[{title: 'list-item'}],
                title: 'Ventas'
            },
            {
                action: 'mdi-account-multiple',
                active: true,
                items:[
                    {title:'Colaboradores'},
                    {title:'Planilla de pago'},
                    ],
                title: 'Personas'
            },
            {
                action: 'mdi-warehouse',
                items:[
                    {title:'list-items'}
                    ],
                title: 'Almacenes'
            },
            {
                action: 'mdi-table-arrow-up',
                items:[
                    {title:'list-items'}
                    ],
                title: 'Alta Dirección'
            },

            
        ]
    })
}
</script>

<style scoped>
.v-list-item__title {
    color: black;
}
.marcado{
    height: 21px;
    border: 2px solid #7B0081;
    position: absolute;
    top: 65px;
    right: -23px;
    background:#7B0081;
}
</style>

