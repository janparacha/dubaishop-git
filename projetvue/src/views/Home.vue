<template>
  <Grille/>
  <MainHome />
</template>

<script>
// @ is an alias to /src
import MainHome from "../components/MainHome.vue";
import Grille from '../components/Grille.vue'

export default {
  name: "Home",
  components: {
    MainHome, Grille,
  },
};
</script>
