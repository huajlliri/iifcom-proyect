<template>
  <v-app>
    
      <AppBar />
      <div id="app">
        <router-view/>
      </div>
      <FooterBar/>
   
  </v-app>
</template>

<script>
import AppBar from './components/AppBar.vue'
import FooterBar from './components/FooterBar.vue';
export default {
  name: 'App',

  data: () => ({
    //
  }),

  components: {
    AppBar,
    FooterBar,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  background-color: #F2FAFF;
  /* margin-top: 60px; */
  line-height: 2;

}

li {
  margin-left: 40px;
}

#style-title {
  white-space: normal;
  font-weight: bold;
  font-size: 1.5em;
}
#card-style {
  line-height: 2;
}
</style>
