<template >
  <v-row class="lighten_grey pl-2" >
    <v-container fluid>
      <v-dialog v-model="dialog" width="600">
        <template v-slot:activator="{ on, attrs }">
          <v-row no-gutters v-bind="attrs" v-on="on" class="pb-2">
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <div class="text-center">
                <p class="font-weight-bold title-detalle">Nombre</p>
              </div>
              <v-card class="rounded-lg pad-5" max-width="280" outlined>
                <div class="row">
                  <v-col cols="3" class="pr-0 pb-0">
                    <v-badge dot bordered overlap bottom color="gree_kit">
                      <v-avatar size="50" class="pl-2">
                        <v-img
                          src="https://cdn.vuetifyjs.com/images/john.png"
                        ></v-img>
                      </v-avatar>
                    </v-badge>
                  </v-col>
                  <v-col class="mr-auto pb-0" cols="9">
                    <p class="mb-0 title">Esteban Quito</p>
                    <p class="text--disabled">Gerente de Finanzas</p>
                  </v-col>
                </div>

                <v-card-actions class="pt-0 pb-3">
                  <v-row class="px-4">
                    <v-col cols="6" sm="6" md="6" class="pa-0">
                      Rendimiento
                    </v-col>
                    <v-col cols="6" sm="6" md="6" class="pa-0 text-right">
                      80%
                    </v-col>
                    <v-col cols="12" sm="12" md="12" class="pa-0">
                      <v-progress-linear
                        color="green accent-3"
                        rounded
                        value="80"
                        height="7"
                      ></v-progress-linear>
                    </v-col>
                  </v-row>
                </v-card-actions>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <div class="text-center">
                <p class="font-weight-bold title-detalle">Jornada</p>
              </div>

              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Tardanzas</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Suspensión</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Horas de trabajos</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <div class="text-center">
                <p class="font-weight-bold title-detalle">Pagos</p>
              </div>
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Ingresos</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Descuento</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Pagar</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <div class="text-center">
                <p class="font-weight-bold title-detalle">Seguros</p>
              </div>
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Seguros</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong> Contribuciones</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Total</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
          </v-row>
          <br />
          <v-row no-gutters class="pb-2">
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card class="rounded-lg pad-5" max-width="280" outlined>
                <div class="row">
                  <v-col cols="3" class="pr-0 pb-0">
                    <v-badge dot bordered overlap bottom color="gree_kit">
                      <v-avatar size="50" class="pl-2">
                        <v-img
                          src="https://cdn.pixabay.com/photo/2014/01/03/01/13/woman-237871_960_720.jpg"
                        ></v-img>
                      </v-avatar>
                    </v-badge>
                  </v-col>
                  <v-col class="mr-auto pb-0" cols="9">
                    <p class="mb-0 title">Elba Ranco</p>
                    <p class="text--disabled">Gerente de Finanzas</p>
                  </v-col>
                </div>

                <v-card-actions class="pt-0 pb-3">
                  <v-row class="px-4">
                    <v-col cols="6" sm="6" md="6" class="pa-0">
                      Rendimiento
                    </v-col>
                    <v-col cols="6" sm="6" md="6" class="pa-0 text-right">
                      80%
                    </v-col>
                    <v-col cols="12" sm="12" md="12" class="pa-0">
                      <v-progress-linear
                        color="orange darken-1"
                        rounded
                        value="80"
                        height="7"
                      ></v-progress-linear>
                    </v-col>
                  </v-row>
                </v-card-actions>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Tardanzas</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Suspensión</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Horas de trabajos</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Ingresos</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Descuento</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Pagar</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Seguros</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong> Contribuciones</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Total</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
          </v-row>

          <v-row no-gutters class="pb-2">
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card class="rounded-lg pad-5" max-width="280" outlined>
                <div class="row">
                  <v-col cols="3" class="pr-0 pb-0">
                    <v-badge dot bordered overlap bottom color="red">
                      <v-avatar size="50" class="pl-2">
                        <v-img
                          src="https://cdn.pixabay.com/photo/2014/01/03/01/13/woman-237871_960_720.jpg"
                        ></v-img>
                      </v-avatar>
                    </v-badge>
                  </v-col>
                  <v-col class="mr-auto pb-0" cols="9">
                    <p class="mb-0 title">Elda ranko</p>
                    <p class="text--disabled">Gerente de Finanzas</p>
                  </v-col>
                </div>

                <v-card-actions class="pt-0 pb-3">
                  <v-row class="px-4">
                    <v-col cols="6" sm="6" md="6" class="pa-0">
                      Rendimiento
                    </v-col>
                    <v-col cols="6" sm="6" md="6" class="pa-0 text-right">
                      47%
                    </v-col>
                    <v-col cols="12" sm="12" md="12" class="pa-0">
                      <v-progress-linear
                        color="red"
                        rounded
                        value="40"
                        height="7"
                      ></v-progress-linear>
                    </v-col>
                  </v-row>
                </v-card-actions>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Tardanzas</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Suspensión</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Horas de trabajos</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Ingresos</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Descuento</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Pagar</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Seguros</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong> Contribuciones</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Total</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
          </v-row>

          <v-row no-gutters class="pb-2">
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card class="rounded-lg pad-5" max-width="280" outlined>
                <div class="row">
                  <v-col cols="3" class="pr-0 pb-0">
                    <v-badge dot bordered overlap bottom color="gree_kit">
                      <v-avatar size="50" class="pl-2">
                        <v-img
                          src="https://cdn.vuetifyjs.com/images/john.png"
                        ></v-img>
                      </v-avatar>
                    </v-badge>
                  </v-col>
                  <v-col class="mr-auto pb-0" cols="9">
                    <p class="mb-0 title">Esteban Quito</p>
                    <p class="text--disabled">Gerente de Finanzas</p>
                  </v-col>
                </div>

                <v-card-actions class="pt-0 pb-3">
                  <v-row class="px-4">
                    <v-col cols="6" sm="6" md="6" class="pa-0">
                      Rendimiento
                    </v-col>
                    <v-col cols="6" sm="6" md="6" class="pa-0 text-right">
                      80%
                    </v-col>
                    <v-col cols="12" sm="12" md="12" class="pa-0">
                      <v-progress-linear
                        color="green accent-3"
                        rounded
                        value="80"
                        height="7"
                      ></v-progress-linear>
                    </v-col>
                  </v-row>
                </v-card-actions>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Tardanzas</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Suspensión</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Horas de trabajos</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="blue" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Ingresos</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="red" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong>Descuento</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="green accent-3" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Pagar</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6" lg="3" xl="3">
              <v-card
                class="d-flex justify-center rounded-lg"
                max-width="280"
                outlined
              >
                <v-list>
                  <v-list-item-group>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >0</span
                          >
                        </v-chip>
                        <strong>Seguros</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 21px !important;
                              margin-left: 21px !important;
                            "
                            >1</span
                          >
                        </v-chip>
                        <strong> Contribuciones</strong>
                      </div>
                    </v-list-item>
                    <v-list-item style="min-height: 30px">
                      <div>
                        <v-chip class="ma-2" color="grey lighten-2" x-small>
                          <span
                            style="
                              margin-right: 15px !important;
                              margin-left: 15px !important;
                            "
                            >104</span
                          >
                        </v-chip>
                        <strong>Total</strong>
                      </div>
                    </v-list-item>
                  </v-list-item-group>
                </v-list>
              </v-card>
            </v-col>
          </v-row>
        </template>
        <v-overlay :absolute="absolute" :opacity="opacity" :color="color">
          <v-card width="700" light>
              <div style="display: flex;
                justify-content: flex-end;
                margin-right: 20px; padding-top:10px">
                 <v-icon @click="dialog = false" size="20px!important" >
                    mdi-close-circle-outline
                </v-icon></div>
            <v-toolbar flat prominent height="200px">
                
              <template>
                   
                <v-row>
                   
                  <v-col cols="3">
                      <v-progress-circular
                        :rotate="-90"
                        :value="80"
                        color="gree_kit"
                        :size="120"
                        :width="11"
                        rounded
                        >
                        <v-avatar size="100" >
                        <v-img
                          src="https://cdn.vuetifyjs.com/images/john.png"
                        ></v-img>
                      </v-avatar>
                        </v-progress-circular>
                   
                    <p> <v-avatar
                        color="gree_kit"
                        size="15"
                        ></v-avatar> 80% Rendimiento</p>
                  </v-col>
                 
                    <v-col class="mr-auto pb-0 pt-7" cols="9">
                        <p class="mb-1 title">Esteban Quito</p>
                        <p class="mb-1 text--disabled">Gerente de Finanzas</p>
                        <p class="mb-1 text--disabled">esteban@gmail.com</p>
                        <p class="mb-1 text--disabled">(306) 555-0121</p>
                        <p class="mb-1 text--disabled">RUC: 0912345678</p>
                    </v-col>
                 
                </v-row>
              </template>

              <template v-slot:extension>
                <v-tabs v-model="tab" align-with-title grow>
                  <v-tabs-slider color="deep-purple"></v-tabs-slider>

                  <v-tab v-for="item in items" :key="item" class="text-capitalize">
                    {{ item }}
                  </v-tab>
                </v-tabs>
              </template>
            </v-toolbar>

            <v-tabs-items v-model="tab" class="py-3">
              <v-tab-item>
                  <p  class="text-center deep-purple--text   text--lighten-1">Del 01 julio al 15 julio 2020</p>
                <div flat>
                  <v-row class="justify-center">
                    <v-card
                      elevation="2"
                      outlined
                      max-width="170px"
                      max-height="250px"
                      class="mr-3"
                    >
                      <v-card-title class="headline grey lighten-2 pa-1">
                        <span class="mx-auto">Jornada</span>
                      </v-card-title>
                      <v-card-text class="pt-3">
                        <strong>07:30 horas ordinarias</strong> <br>
                        <strong>13:00 horas extras 25%</strong> <br>
                        <strong>03:00 horas extras 35%</strong> <br>
                        <strong>00:00 horas feriados</strong> <br>
                        <strong>00:30 permiso</strong> <br>
                        <strong>0 tardanzas</strong> <br>
                        <strong>1 suspensiòn</strong> <br>
                        <div class="text-center pt-6">
                            <p class="mb-1 green--text text--accent-3 font-weight-bold size-f">104:00 HORAS</p>
                            <v-btn
                            color="blue darken-1 white--text"
                            depressed
                            elevation="2"
                            raised
                            rounded
                            >Detalles
                            </v-btn>
                        </div>
                        
                      </v-card-text>
                    </v-card>
                    <v-card
                      elevation="2"
                      outlined
                      max-width="400px"
                      class="mr-3"
                    >
                      <v-card-title class="grey lighten-2 pa-1">
                        <span class="mx-auto">Pago</span>
                      </v-card-title>
                      <v-card-text>
                          <div class="d-flex justify-center px-2 pt-3">
                              <div class="mr-4">
                                    <strong class="green--text text--accent-3">(+) INGRESOS</strong> <br>
                                    <strong>13:00 horas extras 25%</strong> <br>
                                    <strong>13:00 horas extras 25%</strong> <br>
                                    <strong>00:00 horas feriados</strong> <br>
                                    <strong>00:30 permisos</strong> <br>
                                    <strong>0 tardanzas</strong> <br>
                                    <strong>1 suspensiòn</strong> <br>
                                    <strong>00:30 permisos</strong> <br>
                                    <strong>0 tardanzas</strong> <br>
                                    <strong>1 suspensiòn</strong> <br>
                                    <p class="green--text text--accent-3">0.00</p>
                              </div>
                              <div>
                                  <strong class="red--text">(+) DESCUENTOS</strong> <br>
                                   <strong>13:00 horas extras 25%</strong> <br>
                                    <strong>13:00 horas extras 25%</strong> <br>
                                    <strong>00:00 horas feriados</strong> <br>
                                    <strong>00:30 permisos</strong> <br>
                                    <strong>0 tardanzas</strong> <br>
                                    <strong>1 suspensiòn</strong> <br>
                                    <strong>00:30 permisos</strong> <br>
                                    <strong>0 tardanzas</strong> <br>
                                    <strong>1 suspensiòn</strong> <br>
                                    <p class="red--text">0.00</p>
                              </div>
                                
                          </div>
                          <div class="text-center pt-6">
                            <p class="green--text text--accent-3 font-weight-bold size-f">s/633.03</p>
                            <p class="font-weight-medium">PAGADO</p>
                          </div>
                      </v-card-text>
                    </v-card>
                    <v-card elevation="2" outlined max-width="170px" max-height="170px">
                      <v-card-title class="grey lighten-2 pa-1">
                        <span class="mx-auto">Seguros</span>
                      </v-card-title>
                      <v-card-text class="pt-3">
                        <strong>13:00 horas extras 25%</strong> <br>
                        <strong>13:00 horas extras 25%</strong> <br>
                        <strong>00:00 horas feriados</strong> <br>
                        <strong>00:30 permisos</strong> <br>
                        <div class="text-center pt-6">
                            <p class="green--text text--accent-3 font-weight-bold size-f">s/633.03</p>
                        </div>
                      </v-card-text>
                    </v-card>
                  </v-row>
                </div>
              </v-tab-item>
              <v-tab-item>
                <v-card flat>
                  <v-card-title class="headline">
                    An awesome title
                  </v-card-title>
                  <v-card-text>
                    <p>
                      Duis lobortis massa imperdiet quam. Donec vitae orci sed
                      dolor rutrum auctor. Vestibulum facilisis, purus nec
                      pulvinar iaculis, ligula mi congue nunc, vitae euismod
                      ligula urna in dolor. Praesent congue erat at massa.
                    </p>

                    <p>
                      Aenean posuere, tortor sed cursus feugiat, nunc augue
                      blandit nunc, eu sollicitudin urna dolor sagittis lacus.
                      Pellentesque egestas, neque sit amet convallis pulvinar,
                      justo nulla eleifend augue, ac auctor orci leo non est.
                      Etiam sit amet orci eget eros faucibus tincidunt. Donec
                      sodales sagittis magna.
                    </p>

                    <p class="mb-0">
                      Ut leo. Suspendisse potenti. Duis vel nibh at velit
                      scelerisque suscipit. Fusce pharetra convallis urna.
                    </p>
                  </v-card-text>
                </v-card>
              </v-tab-item>
              <v-tab-item>
                <v-card flat>
                  <v-card-title class="headline">
                    An even better title
                  </v-card-title>
                  <v-card-text>
                    <p>
                      Maecenas ullamcorper, dui et placerat feugiat, eros pede
                      varius nisi, condimentum viverra felis nunc et lorem. Sed
                      hendrerit. Maecenas malesuada. Vestibulum ullamcorper
                      mauris at ligula. Proin faucibus arcu quis ante.
                    </p>

                    <p class="mb-0">
                      Etiam vitae tortor. Curabitur ullamcorper ultricies nisi.
                      Sed magna purus, fermentum eu, tincidunt eu, varius ut,
                      felis. Aliquam lobortis. Suspendisse potenti.
                    </p>
                  </v-card-text>
                </v-card>
              </v-tab-item>
              <v-tab-item>
                <v-card flat>
                  <v-card-text>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris nisi ut aliquip ex ea commodo consequat.
                  </v-card-text>
                </v-card>
              </v-tab-item>
              <v-tab-item>
                <v-card flat>
                  <v-card-text>
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris nisi ut aliquip ex ea commodo consequat.
                  </v-card-text>
                </v-card>
              </v-tab-item>
            </v-tabs-items>
          </v-card>
        </v-overlay>
      </v-dialog>
    </v-container>
  </v-row>
</template>
<script>
export default {
  name: "ModalDetalle",
  data() {
    return {
      dialog: false,
      absolute: true,
      opacity: 1,
      color: "rgb(136, 132, 132, 0.99)",
      tab: null,
      items: ["Planillas", "Vacaciones", "Contratos", "Boletos", "Más"],
    };
  },
};
</script>

<style scoped>
.pad-5 {
  padding: 5px;
}
.v-progress-circular {
  margin: 2rem;
}
.size-f{
    font-size: 15px!important;
}

.title-detalle{
    font-size: 13px!important;
}
</style>
