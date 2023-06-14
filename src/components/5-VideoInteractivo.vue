<template>
    <div class="video">
      <p class="video-interactivo">Video Interactivo</p>
  
      <video id="main-video" class="frame-7" :autoplay="opcionSeleccionada !== 0" controls @ended="mostrarBotones">
        <source v-for="(item, index) in videoArray" :key="index" :src="'https://uristotelescep.github.io/media/' + item[1]" type="video/mp4">
      </video>
      
      <div v-show="showOverlay" class="video-overlay">
        <div style="position: relative;">
          <div class="frame-13">
            <div class="flex-wrapper-two">
              <p class="elige-una-opcion">Elige una opción:</p>
              <div class="frame-22" @click="recargarVideo">
                <div class="restart-7-1">
                  <img alt="" class="vector" src="https://static.overlay-tech.com/assets/c11d0502-09a7-43d1-aa80-f7e80cadc0b2.svg" />
                </div>
              </div>
            </div>
            <div class="frame-18">
              <div v-for="(item, index) in videoArray[opcionSelecionada][2]" :key="index" class="frameopciones" @click="cambiarvideo(item)">
                <p class="opciones">
                  {{ videoArray[item][0] }}
                </p>
              </div>
            </div>
            <div v-if="opcionSelecionada !== 0" class="frame-19" @click="irAPreguntaAnterior">
              <p class="pregunta-anterior">Pregunta anterior</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Video-int",
    data() {
      return {
        showOverlay: false,
        showVideo: false,
        opcionSelecionada: 0,
        VideoElement: {},
        videoArray: [
          ["Base", "introGeneral.mp4", [1, 2]],
          ["Estudios", "estudiosBase.mp4", [3, 4]],
          ["Sobre Mi", "introAboutMemp4.mp4", [9, 10]],
          ["Desarollo Multiplataforma", "baseMulti.mp4", [5, 6]],
          ["Desarollo Web", "webBase.mp4", [7, 8]],
          ["Mis preferencias", "preferenciasMulti.mp4"],
          ["Proyectos", "proyectosMulti.mp4"],
          ["Mis preferencias", "preferenciasWeb.mp4"],
          ["Proyectos", "proyectosWeb.mp4"],
          ["Puntos fuertes y puntos flacos", "PuntosMalos.mp4"],
          ["Aficiones", "Aficiones Intro.mp4", [11, 12]],
          ["Simuladores", "simuladores.mp4"],
          ["Musica", "musica.mp4"],
        ],
      };
    },
    created() {
      let cont = this;
      window.addEventListener("DOMContentLoaded", () => {
        cont.VideoElement = document.getElementById("main-video");
      });
    },
    computed: {
        PreguntaAnterior()
        {
            switch(this.opcionSelecionada)
            {
                case 11:
                case 12:
                    return 10;
                
                case 7:
                case 8:
                    return 4;
                
                case 5:
                case 6:
                    return 3;
                
                case 9:
                case 10:
                    return 2;
                
                case 3:
                case 4:
                    return 1;
                
                case 1:
                case 2:
                    return 0;
                
                
            }
            return -1;
        }
    },
    methods: {
        irAPreguntaAnterior() {
    const preguntaAnterior = this.PreguntaAnterior;
    if (preguntaAnterior !== -1) {
      this.opcionSelecionada = preguntaAnterior;
      
    }
  },
      opcionSeleccionada() {
        let video = document.getElementById("main-video");
        video.src = 'https://uristotelescep.github.io/media/' + this.videoArray[this.opcionSelecionada][1];
        video.load();
      },
      cambiarvideo(num) {
        this.showVideo = true;
        this.opcionSelecionada = num;
        this.opcionSeleccionada();
        this.showOverlay = false;
      },
      recargarVideo() {
        let video = document.getElementById("main-video");
        video.load();
        this.showOverlay = false;
      },
      mostrarOverlay() {
        this.showOverlay = true;
      },
      mostrarBotones() {
        this.showVideo = false;
        this.showOverlay = true;
      },
    },
  };
  </script>
<style lang="scss" scoped>
@import "/src/Estilos.scss";

.video {
    background-color: rgba(255, 255, 255, 1);
    padding: 56px 314px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.video-interactivo {
    color: $blue;
    margin-bottom: 85px;
    @include inter-64-extra-light;
}

.frame-7 {
    background-color: rgba(217, 217, 217, 1);
    border-radius: 20px;
    width: 80%;
    display: flex;
    align-items: center;

    border: 4px solid $blue;
}

.play-button-svgrepo-com-1 {
    padding: 9px 19px 8px;
    position: relative;
}

.ellipse-3 {
    width: 172px;
    height: 172px;
    background-color: $blue;
    border-radius: 50%;
    position: relative;
    border: 1px solid $blue;
}



.video-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: rgba(0, 0, 0, 0.5);
    color: #ffffff;
    font-size: 24px;
    z-index: 13;
}

@import "/src/Estilos.scss";

.frame-13 {
    background-color: rgba(241, 241, 241, 0.938);
    border-radius: 20px;
    padding: 17px 131px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

}

.flex-wrapper-two {
    margin-bottom: 38px;

    display: flex;
    align-items: flex-start;
}

.elige-una-opcion {
    height: 91px;
    width: 678px;
    font-family: "Inter";
    font-size: 48px;
    font-weight: 700;
    line-height: normal;
    color: $blue;
    display: flex;
    align-items: center;
    text-align: center;
    margin-top: 32px;
    justify-content: center;
}

.frame-22 {
    background-color: $blue;
    border-radius: 50%;
    padding: 14px 14px 14px 13px;
    position: absolute;
    top: 2%;
    right: 2%;
}

.restart-7-1 {
    padding: 0 0.04px 0 0;
    display: flex;
    align-items: flex-start;
    flex: 1;
    align-self: stretch;
}

.vector {}

.frame-18 {
    margin-bottom: 38px;
    display: flex;
    align-items: flex-start;

}

.frameopciones {
    background-color: $green;
    border-radius: 15px;
    display: flex;

    align-items: flex-start;

    &:not(:last-of-type) {
        margin-right: 236px;
    }
}

.opciones {
    height: 143px;
    width: 352px;
    font-family: "Inter";
    font-size: 36px;
    font-weight: 900;
    line-height: normal;
    color: rgba(255, 255, 255, 1);
    display: flex;
    align-items: center;
    text-align: center;
    justify-content: center;
}

.frame-19 {

    border-radius: 15px;
    display: flex;
    align-items: center;
    background: $blue;
    ;
    width: 352px;
}

.pregunta-anterior {
    height: 143px;
    width: 352px;
    font-family: "Inter";
    font-size: 36px;
    font-weight: 900;
    line-height: normal;
    color: rgb(212, 212, 212);
    display: flex;
    align-items: center;
    text-align: center;
    justify-content: center;
}</style>
  