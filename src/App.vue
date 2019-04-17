<template>
  <v-app class="grey lighten-4">
    <Navabar-app></Navabar-app>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import Navabar from "./components/Navbar";

export default {
  name: "App",
  components:{
      NavabarApp:Navabar
  },
  data() {
    return {
      //
    };
  }
};
</script>
