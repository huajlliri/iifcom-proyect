<template>
    <v-container>
      <v-carousel cycle  hide-delimiter-background show-arrows="hover">
      <v-carousel-item v-for="(slide, i) in slides" :key="i"
         :src="images[i]" cover>
      </v-carousel-item>
    </v-carousel>
    </v-container>
  </template>
  
  <script>
    export default {
      data() {
        return {
          images: [
            'https://st5.depositphotos.com/64145070/64693/i/450/depositphotos_646930840-stock-photo-sunset-ocean-beach-beautiful-seascape.jpg',
            'https://imagenes.muyinteresante.es/files/composte_image/uploads/2023/08/01/64c8a20035395.jpeg',
            'https://st2.depositphotos.com/1004017/6338/v/450/depositphotos_63386971-stock-illustration-tropical-island-with-palm-trees.jpg',
            'https://m.media-amazon.com/images/I/71ETAmGMIsL.jpg',
            'https://st3.depositphotos.com/1105977/16920/i/450/depositphotos_169209040-stock-photo-beautiful-autumn-scenery-in-park.jpg',
            'https://pics.craiyon.com/2023-07-07/0058aa5a11a94a1ba91b80c8c295ceeb.webp',
          ],
          slides: ['uno', 'dos', 'tres', 'cuatro', 'cinco', 'seis'],
        }
      },
    }
  </script>
  