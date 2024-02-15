<template>
    <v-app-bar scroll-behavior="hide">
        <v-toolbar color="#F2FAFF">
            <router-link :to="{ name: 'home' }">
                <v-img class="ms-8" :width="100" src="../assets/logo-iifcom.png"></v-img>
            </router-link>

            <v-spacer></v-spacer>

            <v-toolbar-items>
                <v-btn variant="text" to="service" class="hidden-sm-and-down">Nuestros Servicios</v-btn>

                <v-divider vertical class="hidden-sm-and-down"></v-divider>

                <v-btn variant="text" to="about" class="hidden-sm-and-down">Conócenos</v-btn>
            </v-toolbar-items>

            <v-divider vertical></v-divider>

            <v-menu transition="scale-transition">
                <template v-slot:activator="{ props }">
                    <v-app-bar-nav-icon class="ms-2 hidden-md-and-up" v-bind="props"></v-app-bar-nav-icon>
                </template>
                <v-list>
                    <v-list-item v-for="(menu, i) in menus" :key="i">
                        <router-link :to="{ name: menu.name }" class="decoration">
                            <v-list-item-title>{{ menu.title }}</v-list-item-title>
                        </router-link>
                    </v-list-item>
                </v-list>
            </v-menu>
        </v-toolbar>
    </v-app-bar>
</template>
  
<script setup>

const menus = [
    { title: 'Nuestros Servicios', name: 'service' },
    { title: 'Conócenos', name: 'about' },
]
</script>
  
  
  
<style scoped>
.decoration {
    text-decoration: none;
    color: inherit;
}
</style>
  