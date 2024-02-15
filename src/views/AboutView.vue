<template>
  <br>
  <div>
    <row align="center" no-gutters>
      <v-card>
        <div class="background-img">
          <h1>IIFCOM</h1>
          <h4>(Ingeniería e Infraestructura para Sistemas de Comunicación)</h4>
        </div>
      </v-card>


    </row>
    <v-row align="center" class="justify-center pa-4" style="background-color: rgb(181, 226, 255);">
      <v-col cols="auto" sm="6">
        <v-card color="transparent" variant="flat">

          <v-card-title id="style-title">
            Misión
          </v-card-title>

          <v-card-text id="card-style">
            Crear soluciones integrales en telecomunicaciones, proveyendo a nuestros clientes servicios tecnológicos
            innovadores de alta calidad a través del trabajo especializado de nuestro personal y de la gestión y
            adquisición
            de tecnología vanguardista.
          </v-card-text>

        </v-card>
      </v-col>
      <v-col cols="auto" sm="6">
        <v-card color="transparent" variant="flat">

          <v-card-title id="style-title">
            Nuestros Servicios
          </v-card-title>


          <v-card-text id="card-style">
            En IIFCOM, nos especializamos en brindar servicios de alta calidad
            en el ámbito de las telecomunicaciones. Nuestra oferta de servicios
            abarca una amplia gama de soluciones para satisfacer las necesidades
            de nuestros clientes.
          </v-card-text>

        </v-card>
      </v-col>
    </v-row>

    <v-row justify="center">
      <v-col cols="12" class="text-center ma-8">
        <h1>¿Por qué elegir IIFCOM?</h1>
      </v-col>
    </v-row>

    <v-row align="center" justify="center">
      <v-col v-for="(item, index) in items" :key="index" cols="auto">
        <v-card class="transparent-card">
          <v-img class="custom-image" :src="require(`@/assets/${item.imageSrc}`)">
            <template v-slot:placeholder>
              <v-row class="fill-height ma-0" align="center" justify="center">
                <v-progress-circular indeterminate color="grey-lighten-5" ></v-progress-circular>
              </v-row>
            </template>
          </v-img>
          <div class="d-flex justify-center">
            <h3>{{ item.title }}</h3>
          </div>
        </v-card>
      </v-col>
    </v-row>



    <v-row class="justify-center pa-4 flex-wrap-reverse">
      <v-col cols="auto">
        <v-card variant="flat" color="transparent">
          <v-card-title id="style-title">Nuestro Protocolo de Desarrollo</v-card-title>
          <v-card-subtitle>
            para completar cada proyecto <br> con plena satisfacción es:
          </v-card-subtitle>
          <ul>
            <li>Diseño del proyecto a realizar</li>
            <li>Instalación y programación</li>
            <li>Verificación del funcionamiento</li>
            <li>Capacidad de personal</li>
            <li>Mantenimiento y servicio</li>
            <li>Consultoría</li>
          </ul>
        </v-card>
      </v-col>
      <v-col cols="auto">
        <v-img class="custom-image" :width="400" src="../assets/grupo-trabajo.jpg">
          <template v-slot:placeholder>
            <v-row class="fill-height ma-0" align="center" justify="center">
              <v-progress-circular indeterminate color="grey-lighten-5"></v-progress-circular>
            </v-row>
          </template>
        </v-img>
      </v-col>
    </v-row>
  </div>
  <br>
</template>

<script setup>
const items = [
  { title: 'Calidad', imageSrc: 'calidad.png' },
  { title: 'Eficiencia', imageSrc: 'eficiencia.png' },
  { title: 'Puntualidad', imageSrc: 'reloj.png' }
];
</script>


<style scoped>
.custom-image {
  height: 250px;
  width: 300px;
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.background-img {
  padding: 60px;
  position: relative;
}

.background-img::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('../assets/fondo1.jpg');
  background-size: cover;
  /* background-position: center; */
  opacity: 0.5;

}

.background-img h1,
h4 {
  position: relative;
  z-index: 1;
  text-align: center;
}

.transparent-card {
  background-color: transparent;
  box-shadow: 0px 0px 10px 2px rgba(143, 188, 209, 0.781);
  border: 2px solid rgb(181, 226, 255);
  border-radius: 8px;
}
</style>