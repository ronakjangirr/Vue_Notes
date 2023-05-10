<template>
    <div>

        <v-container >
            <v-row class="d-flex justify-end pa-3">
            <v-col cols="12">
                <v-select label="Select" :items="['POSITION', 'PRODUCT NAME', 'PRICE:LOW-HIGH', 'COLOR']"
                    variant="outlined">
                </v-select>
            </v-col>
            </v-row>
        </v-container>

        <v-container fluid>
            <v-row class="d-flex justify-space-around">
                <v-col cols="4">

                    <v-row justify="center">
                        <v-expansion-panels accordion>
                            <v-expansion-panel>
                                <v-expansion-panel-header>BRAND</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                            <v-expansion-panel>
                                <v-expansion-panel-header>DESIGN STYLE</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                            <v-expansion-panel>
                                <v-expansion-panel-header>OCCASSION</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                            <v-expansion-panel>
                                <v-expansion-panel-header>PAPER COLOR</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                            <v-expansion-panel>
                                <v-expansion-panel-header>PAPER WEIGHT</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                            <v-expansion-panel>
                                <v-expansion-panel-header>PHOTO CARD</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                            <v-expansion-panel>
                                <v-expansion-panel-header>PRODUCT TYPE</v-expansion-panel-header>
                                <v-expansion-panel-content>
                                  <ul>
                                    <li>Crane</li>
                                    <li>Train</li>
                                  </ul>
                                </v-expansion-panel-content>
                            </v-expansion-panel>
                        </v-expansion-panels>
                    </v-row>

                </v-col>
                <v-col cols="8">

                </v-col>
            </v-row>
        </v-container>

    </div>
</template>

<script>
export default {
    name: "MiddleVue"
}

</script>

<script>


</script>