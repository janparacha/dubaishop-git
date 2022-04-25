<template>
    <Header/>
  <div id="nav">
    <nav>
            <ul class="navdekstop">
                <li> <router-link to="/"> Accueil</router-link> </li>
                <li> <router-link to="/parfum"> Parfum</router-link>
                    <div class="sub-menu1">
                    <ul>
                        <li><a href="#">Collection Lataffa</a> </li>
                        <li><a href="#"> Musk</a> </li> 
                    </ul>
                    </div>
                </li>
                <li><a href="#">Désodorisants</a> </li>
                <li><a href="#">Bougies </a>
                    <div class="sub-menu1">
                    <ul>
                        <li> <a href="#"> Karamat </a> </li>
                        <li> <a href="#"> Encens </a> </li> 
                    </ul>
                    </div>
                </li>
                <li><a href="#"> Vetements femme </a></li>
                <li><a href="#"> Bijoux </a></li>
                <li><a href="#"> Nous contacter </a></li>
            </ul>
        </nav>
    </div>
    <router-view/>
  <Footer />
</template>

<script>
import Header from "./components/Header.vue"
import Footer from "./components/Footer.vue"

export default {
  name: "app",
  components: 
  {
    Header,Footer,
  },
}
</script>

<style lang='scss'>
@import '../../style.scss';


#app {
  font-family: "Domine",Arial, Helvetica, sans-serif;
  font-size: 1em;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;

    &.router-link-exact-active {
      color: #d8a12c;
    }
  }
}
</style>
