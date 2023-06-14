<template>
  <div>
    <div class="navBase">
      <!-- Videoint -->
      <div class="navVideo" @click="scrollToComponent('videoInteractivo')">Video Interactivo</div>
      <!-- Sobremi -->
      <div class="navsobreMi" @click="scrollToComponent('aboutMe')">Sobre Mi</div>
      <!-- Logo e inicio -->
      <div class="navLogo">
        <img alt="" src="https://static.overlay-tech.com/assets/4eee9806-7473-44b7-8ca5-e8c4bcad89dc.svg" />
        <div class="uristoteles">Uristóteles</div>
      </div>
      <!-- Manual -->
      <div class="navManual" @click="scrollToComponent('manualIdentidad')">Manual de Identidad</div>
      <!-- Proyectos recientes -->
      <div class="navProyectos" @click="scrollToComponent('misProyectos')">Proyectos recientes</div>
    </div>

    <Intro ref="videoInteractivo"></Intro>
    <AboutMe ref="aboutMe"></AboutMe>
    <ManualIdentidad ref="manualIdentidad"></ManualIdentidad>
    <MisProyectos ref="misProyectos"></MisProyectos>
    <VideoInteractivo ref="videoInteractivo"></VideoInteractivo>
  </div>
</template>

<script>
import Intro from './components/1-Intro.vue'
import AboutMe from './components/2-AboutMe.vue'
import ManualIdentidad from './components/3-ManualIdentidad.vue'
import MisProyectos from './components/4-MisProyectos.vue'
import VideoInteractivo from './components/5-VideoInteractivo.vue'

export default {
  name: 'App',
  components: {
    Intro,
    AboutMe,
    ManualIdentidad,
    MisProyectos,
    VideoInteractivo
  },
  methods: {
    scrollToComponent(refName) {
      const component = this.$refs[refName];
      if (component) {
        component.$el.scrollIntoView({ behavior: 'smooth' });
      }
    }
  }
}
</script>

<style>
.navBase {
  position: sticky;
  top: 0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  height: 109px;
  min-height: 60px; /* Ajusta la altura mínima según tus necesidades */
  background: #F1F1F1;
  z-index: 10;
}

.navVideo,
.navsobreMi,
.navLogo,
.navManual,
.navProyectos {
  font-family: 'Inter';
  font-style: normal;
  font-weight: 300;
  font-size: 32px;
  line-height: 39px;
  display: flex;
  align-items: center;
  text-align: center;
  /* blue */
  color: #34495E;
  
}
.navManual{
  width: 160px;
}
.navLogo {
  display: flex;
  flex-direction: column;
  align-items: center;
  
}

.navLogo img {
  max-height: 70px; /* Ajusta el tamaño del logo según tus necesidades */
}

.navLogo .uristoteles {
  font-family: 'Jura';
  
}
</style>
