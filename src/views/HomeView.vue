<template>
  <div>
    <CarouselView />
    <br>

    <v-row align="center" class="justify-center pa-4" style="background-color: rgb(181, 226, 255);">
      <v-col cols="auto">
        <v-card variant="flat" color="transparent" max-width="600">

          <v-card-title id="style-title">
            Nuestros Servicios
          </v-card-title>
          <v-card-subtitle>
            Servicios que ofrecemos a nuestros clientes
          </v-card-subtitle>

          <v-card-text style="line-height: 2;">
            En IIFCOM, nos especializamos en brindar servicios de alta calidad
            en el ámbito de las telecomunicaciones. Nuestra oferta de servicios
            abarca una amplia gama de soluciones para satisfacer las necesidades
            de nuestros clientes.
          </v-card-text>
          <v-card-actions class="justify-end ma-0">
            <v-btn to="service" variant="outlined"> Ver mas... </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
      <v-col cols="auto">
        <v-img class="custom-image1" :width="600" src="../assets/protocolo.jpeg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template></v-img>
      </v-col>
    </v-row>

    <v-row align="center" class="flex-wrap-reverse  justify-center pa-4">
      <v-col cols="auto" class="order-2">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">Venta de equipos y accesorios de Telecomunicaciones</v-card-title>

          <ul>
            <li>Provisión de equipamiento para telecomunicaciones. </li>
            <li>Provisión de materiales para redes de telecomunicaciones terrestres.</li>
            <li>Provisión de materiales para redes de telecomunicaciones subterráneas. </li>
            <li>Provisión de materiales para redes de fibra óptica. </li>
            <li>Provisión de materiales para sistemas de vigilancia. </li>
            <li>Provisión de materiales para sistemas eléctricos. </li>
            <li>Provisión de materiales para sistemas eléctricos y SPAT .</li>
            <li>Provisión de materiales para sistemas satelitales.</li>

          </ul>
        </v-card>
      </v-col>
      
      <v-col cols="auto" class="order-1">
        <v-img class="custom-image1" :width="600" src="../assets/accesorios.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>

    </v-row>

    <v-row align="center" class="justify-center pa-4" style="background-color: rgb(181, 226, 255);">
      <v-col cols="auto">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">PRODUCTOS Y SERVICIOS</v-card-title>

          <ul>
            <li>Telecomunicaciones </li>
            <li>Redes Metropolitanas </li>
            <li>Enlaces punto a punto </li>
            <li>Redes LAN </li>
            <li>Cableado Estructurado </li>
            <li>Diseño de redes Wireless </li>
            <li>Sistemas de Seguridad </li>
            <li>Sistemas de CCTV </li>
            <li>Sistemas de Control de Acceso </li>
            <li>Telefonía </li>
            <li>Telefonía Digital </li>
            <li>Telefonía sobre IP </li>

          </ul>
        </v-card>
      </v-col>
      <v-col cols="auto">
        <v-img class="custom-image1" :width="600" src="../assets/accesorios.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>

    <v-row align="center" class="flex-wrap-reverse  justify-center pa-4">
      <v-col cols="auto" class="order-2">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">PRODUCTOS Y SERVICIOS ADICIONALES</v-card-title>

          <ul>
            <li>Diseño lógico de Redes </li>
            <li>Certificación de Redes </li>
            <li>Pólizas de Mantenimiento </li>
            <li>Diseño de redes VPN </li>
            <li>Instalación y Configuración de Servidores </li>
            <li>Instalación y Configuración de Antivirus Corporativo </li>
            <li>Mantenimiento y reparación de Computadoras de escritorio y portátiles.</li>


          </ul>
        </v-card>
      </v-col>
      <v-col cols="auto" class="order-1">
        <v-img class="custom-image1" :width="600" src="../assets/accesorios.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>

    <div class="py-14 text-center" style="background-color: rgb(181, 226, 255);">
      En IIFCOM, no solo ofrecemos productos y servicios;
      brindamos soluciones completas que impulsan el éxito
      y la eficiencia de tu infraestructura de comunicaciones.
    </div>


  </div>
</template>

<script>
import { defineComponent } from 'vue';

import CarouselView from '@/components/CarouselView.vue';

export default defineComponent({
  name: 'HomeView',

  components: {

    CarouselView,
  },
  data: () => ({

  }),
});
</script>


<style scoped>
.custom-image1 {
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
