<template>
  <v-footer class="bg-indigo-accent-4  d-flex flex-column">
    <div>
      <v-btn v-for="icon in icons" :key="icon" class="mx-4" :icon="icon" variant="text"></v-btn>
    </div>

    <div>
      <v-row  dense>
        <v-col cols="auto" class="mx-4 px-4">
          <v-card variant="flat" color="transparent">
            <v-card-title id="style-title" class="ma-5">Servicios</v-card-title>
            <ul>
              <li>Fibra Óptica</li>
              <li>Inalámbricas</li>
              <li>Obras civiles</li>
              <li>Cableado estructurado</li>
              <li>Cámaras de Vigilancia</li>
              <li>Sistemas Satelitales</li>
            </ul>
          </v-card>
        </v-col>
        <!-- <v-divider :thickness="3" class="border-opacity-50" color="#B5E2FF" vertical></v-divider> -->
        <v-col cols="auto" class="mx-4 px-4">
          <v-card variant="flat" color="transparent">
            <v-card-title id="style-title" class="ma-5">Información de contacto</v-card-title>
            <v-card-item>
              <v-btn prepend-icon="mdi-email-outline" variant="text">
                test@gmail.com
              </v-btn>
              <br>
              <v-btn prepend-icon="mdi-phone" variant="text">
                99994875
              </v-btn>
            </v-card-item>
          </v-card>
        </v-col>
      </v-row>
    </div>
    <br>
    <div>
      {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
    </div>
    <br>

  </v-footer>
</template>
<script>
export default {
  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-linkedin',
      'mdi-instagram',
    ],
  }),
}
</script>
