<template>
  <v-layout>
    <v-app-bar direction: rtl>

      <v-row style="direction:rtl">

        <!-- <v-col cols="2" class="hidden-md-and-up">
          <v-app-bar-nav-icon @click="this.open = !this.open"></v-app-bar-nav-icon>
        </v-col> -->
        <v-col class="" cols="9" sm="8" md="8" lg="6">
          <v-btn class="bt" style="translate: -10px 20px" color="primary" to="/">الرئيسية </v-btn>
          <v-btn class="bt" style="translate: -10px 20px" to="/quraan"> القرآن الكريم </v-btn>
          <v-btn class="bt" style="translate: -10px 20px"  to="/sm">عن المطور</v-btn>
        </v-col>
        <v-spacer class="hidden-sm-and-down"></v-spacer>>
        <v-col lg="2" md="3" sm="3" cols="2">
          <v-switch style="translate: 0 10px;"
            @change="toggleTheme(); icon == 'mdi-moon-full' ? icon = 'mdi-white-balance-sunny' : icon = 'mdi-moon-full'"
            :prepend-icon="icon"></v-switch></v-col>
        <v-col class="hidden-md-and-down" col="4"></v-col>
      </v-row>
    </v-app-bar>
    <!-- <v-navigation-drawer class="hidden-md-and-up" v-model="this.open">
      <v-switch
        @change="toggleTheme(); icon == 'mdi-moon-full' ? icon = 'mdi-white-balance-sunny' : icon = 'mdi-moon-full'"
        :prepend-icon="icon"></v-switch>
      <v-list>
        <V-list-item to="/quraan" color="primary" value="qr" append-icon="mdi-book">
          القرآن االكريم
        </V-list-item>
      </v-list>
    </v-navigation-drawer> -->
  </v-layout>
  <router-view />
</template>

<style>
@media (max-width:405px) {
  .bt {
    font-size: 10px !important;
    width: 50px
  }
}
</style>

<script>
export default {
  created: function () {
    localStorage.setItem("theme", "light")
  },
  data: function () {
    return {
      open: false,
      icon: ""
    };
  },

};
</script>

<script setup>
import { useTheme } from 'vuetify'

const theme = useTheme()
let icon = "mdi-white-balance-sunny"
function toggleTheme() {
  theme.global.name.value = theme.global.current.value.dark ? 'light' : 'dark';
}

</script>