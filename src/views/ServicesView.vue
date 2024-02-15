<template>
  <br>
  <br>
  <div>

    <v-row justify="center" style="background-color: rgb(181, 226, 255);">
      <v-col class="text-center ma-8">
        <h1>Servicios que ofrecemos a nuestros clientes</h1>
      </v-col>
    </v-row>

    <v-row justify="center" style="background-color: rgb(181, 226, 255);">
      <v-col v-for="(item, index) in items" :key="index" cols="auto">
        <v-card color="transparent" variant="flat">
          <v-img class="custom-image" :src="require(`@/assets/${item.imageSrc}`)">
            <template v-slot:placeholder>
              <v-row class="fill-height ma-0" align="center" justify="center">
                <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
              </v-row>
            </template>
          </v-img>
          <div class="d-flex justify-center">
            <h3>{{ item.title }}</h3>
          </div>
        </v-card>
      </v-col>
    </v-row>


    <div>
      <v-card-title id="style-title" class="ma-5">Fibra Óptica</v-card-title>
      <v-row align="center" justify="center" dense>
        <v-col cols="auto">
          <v-card color="transparent" variant="flat" class="mb-6">
            <v-img :width="400" src="../assets/cable.jpg"></v-img>
            <div class="mb-6">
              <ul>
                <li>Fusiones por arco eléctrico </li>
                <li>Certificaciones con OTDR </li>
                <li>Habilitación de Muflas externas </li>
                <li>Habilitación de Muflas </li>
                <li>Subterráneas </li>
              </ul>
            </div>
          </v-card>

        </v-col>
        <v-col cols="auto">
          <v-card color="transparent" variant="flat" class="mb-6">
            <v-img :width="400" src="../assets/cableado.png"></v-img>
            <div class="mb-6">
              <ul>
                <li>Habilitación de ODF </li>
                <li>Habitación de Patch Panel`s </li>
                <li>Habitación de Pig Tail`s </li>
                <li>Venta de Media Converter`s </li>
                <li>Venta cables Fibra Óptica </li>
              </ul>
            </div>
          </v-card>

        </v-col>

        <v-col cols="auto">
          <v-card color="transparent" variant="flat" class="mb-6">
            <v-img :width="400" src="../assets/accesorios.jpg"></v-img>
            <div class=" mb-6">
              <ul>
                <li>Venta de Patch Cord`s </li>
                <li>Venta de Accesorios de Fibra Óptica </li>
                <li>Venta de Fusionadoras </li>
                <li>Venta de OTDR </li>
                <li>Venta de insumos en fibra Óptica </li>
              </ul>
            </div>
          </v-card>

        </v-col>
      </v-row>
    </div>

    <div style="background-color: rgb(181, 226, 255);">
      <v-card-title id="style-title" class="ma-5">Inalámbricas </v-card-title>
      <v-row justify="center" class="pa-8 ma-2" dense>
        <v-col cols="auto" class="text-center">
          <v-card class="mx-auto" max-width="400">
            <v-img src="../assets/Imagen1.jpg" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px" cover>
              <v-card-title class="text-white">Instalación de antenas sectoriales</v-card-title>
            </v-img>
          </v-card>
        </v-col>
        <v-col cols="auto" class="text-center">
          <v-card class="mx-auto" max-width="400">
            <v-img src="../assets/Imagen3.jpg" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px" cover>
              <v-card-title class="text-white">Mantenimiento de Torres</v-card-title>
            </v-img>
          </v-card>
        </v-col>
        <v-col cols="auto" class="text-center">
          <v-card class="mx-auto" max-width="400">
            <v-img src="../assets/Imagen2.jpg" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px" cover>
              <v-card-title class="text-white">Instalación de sistemas de Pararrayos</v-card-title>
            </v-img>
          </v-card>

        </v-col>

        <v-col cols="auto" class="text-center">
          <v-card class="mx-auto" max-width="400">
            <v-img src="../assets/Imagen4.jpg" class="align-end" gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="400px" cover>
              <v-card-title class="text-white"> Mantenimiento de Antenas</v-card-title>
            </v-img>
          </v-card>
        </v-col>
      </v-row>
    </div>

    <v-row align="center" class="justify-center pa-4">
      <v-col cols="auto">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">Obras civiles</v-card-title>

          <ul>
            <li>Diseño y ejecución de sistemas eléctricos generadores, paneles solares, rectificadores, rack de baterías.
            </li>
            <li>Canalizaciones urbanas para redes de cobre y fibra óptica. </li>
            <li>Canalizaciones rurales larga distancia para redes de cobre y fibra óptica. </li>
            <li>Sistemas de pararrayos.</li>
            <li>Sistemas de puesta a tierra.</li>
            <li>Instalación de cámaras de inspecciones de todo tipo.</li>
            <li>Instalación de bases de armarios para todo tipo.</li>
            <li>Diseño y construcción de Data Center de TIER1, 2, 3.</li>
          </ul>
        </v-card>
      </v-col>


      <v-col cols="auto">
        <v-img class="custom-image2" :width="600" src="../assets/obras.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>

    <v-row align="center" class="flex-wrap-reverse justify-center pa-4"
      style="background-color: rgb(181, 226, 255);">
      <v-col cols="auto" class="order-2">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">Cableado estructurado</v-card-title>

          <ul>
            <li>Instalación de Cableado estructurado Categoria 5E LAN, WAN, MAN.</li>
            <li>Instalación de Cableado estructurado Categoria 6, 6ª, 7, 7ª Ultra.</li>
            <li>Provisión de Materiales de cableado estructurado.</li>
            <li>Venta e instalación de Switch.</li>
            <li>Venta e Instalación de Router`s.</li>
            <li>Venta e instalación de Firewall.</li>
            <li>Venta e instalación de Rack y gabinetes.</li>
            <li>Venta de Accesorios de cableado estructurado.</li>

          </ul>
        </v-card>
      </v-col>
      <v-col cols="auto" class="order-1">
        <v-img class="custom-image2" :width="600" src="../assets/cableado-estructurado.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>

    <v-row align="center" class="justify-center pa-4">
      <v-col cols="auto">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">Cámaras de Vigilancia </v-card-title>

          <ul>
            <li>Diseño de Redes para cámaras de vigilancia para colegios, industrias, oficinas y domicilios </li>
            <li>Instalación de cámaras externa y externa en tecnologías POE IP y NVR </li>
            <li>Instalación de Postes para cámaras exteriores </li>
            <li>Instalación de cámaras de seguridad ciudadana </li>
            <li>Instalación de sistemas de megafonía IP </li>
            <li>Instalación de cámaras ojo de pez </li>
            <li>Instalación de cámaras PTZ </li>
            <li>Instalación de Nodos o gabinetes exteriores </li>
            <li>Venta de cámaras de vigilancia IP POE </li>
            <li>Venta NVR de 8 accesos </li>
            <li>Venta de discos duros para NVR </li>
            <li>Venta de gabinetes para interiores </li>
            <li>Venta de inyectores POE </li>
            <li>Venta de accesorios de conexión para sistemas de video vigilancia </li>
          </ul>
        </v-card>
      </v-col>
      <v-col cols="auto">
        <v-img class="custom-image2" :width="600" src="../assets/camaras.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>


    <v-row align="center" class="flex-wrap-reverse justify-center pa-4"
      style="background-color: rgb(181, 226, 255);">
      <v-col cols="auto" class="order-2">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">Sistemas Satelitales</v-card-title>
          <ul>
            <li>Instalación de antenas satelitales de 1.2 banda KU. </li>
            <li>Instalación de antenas satelitales de 1.8 banda KU. </li>
            <li>Instalación de antenas satelitales de 2.1 banda KU. </li>
            <li>Instalación de Internet satelital de 2 a 30 Mbps. </li>
            <li>Instalación de servicio transmisión de datos. satelital. </li>
            <li>Venta de accesorios satelitales. </li>
            <li>Asesoría en conexiones Satelitales. </li>

          </ul>
        </v-card>
      </v-col>
      <v-col cols="auto" class="order-1">
        <v-img class="custom-image2" :width="600" src="../assets/satelite.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>

const items = [
  { title: 'Instalación de Redes de Terrestres', imageSrc: 'sistemaTierra.jpg' },
  { title: 'Mantenimiento de Redes de Telecomunicaciones', imageSrc: 'mantenimiento_telecomunicaciones.jpg' },
]
</script>

<style scoped>
.custom-image {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 200px;
  border-radius: 20px;
}

.custom-image2 {
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.transparent-card {
  background-color: transparent;
  box-shadow: 0px 0px 10px 2px rgba(229, 244, 252, 0.925);
  border: 2px solid rgb(116, 187, 238);
  border-radius: 8px;
}
</style>