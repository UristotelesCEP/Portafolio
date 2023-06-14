<template>
    <div class="about-me">
      <p class="sobre-mi">Sobre mi</p>
      <div class="frame-10">
        <div class="flex-wrapper-one">
          <p class="empece-a-programas-a-los-16-anos-para-au">
            Empecé a programas a los 16 años para automatizar
            mis deberes de matemáticas y física y le acabe
            pillando el gustillo y bueno, aquí sigo :) <br />
          </p>
          <p class="hoy-en-dia-me-dedico-a-programar-en-web">
            Hoy en dia me dedico a programar en web y algo de
            Android(Java) me siento muy cómodo con JavaScript
            y el framework de VUE.
          </p>
        </div>
        <img
          alt=""
          class="frame-9"
          src="https://static.overlay-tech.com/assets/a8a74a60-e717-4622-bfba-05a042b0967a.svg"
        />
        <div class="flex-wrapper-two">
          <p class="he-estudiado-2-grados-superiores-desarol">
            He estudiado dos grados superiores: Desarollo de
            aplicaciones Multiplataforma y Desarollo de
            aplicaciones WEB
          </p>
          <p
            class="me-considero-programador-full-stack-ya-qu"
          >
            Me considero programador FullStack ya que me gusta
            tanto la parte del backend como la del frontend
          </p>
        </div>
      </div>
      <div class="frame-1">
        <p class="video-interactivo">Video interactivo</p>
      </div>
      <p class="si-deseas-saber-mas-mira-mi-video-intera">
        Si deseas saber mas mira mi video interactivo!
      </p>
    </div>
  </template>
  
  <script>
  export default {
    name: "AboutMe"
  };
  </script>
  
  <style lang="scss" scoped>
  @import "/src/Estilos.scss";
  .about-me {
    background-color: rgba(255, 255, 255, 1);
    padding: 53px 118px 195px 64px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .sobre-mi {
    color: $blue;
    
    @include inter-64-extra-light;
  }
  .frame-10 {
    
    
    display: flex;
    align-items: flex-start;
  }
  .flex-wrapper-one {
    margin-right: 116px;
    padding: 41px 0 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  .empece-a-programas-a-los-16-anos-para-au {
    height: 192px;
    width: 726px;
    color: $blue;
    display: flex;
    text-align: right;
    margin-bottom: 104px;
    @include textos;
  }
  .hoy-en-dia-me-dedico-a-programar-en-web {
    height: 211px;
    width: 726px;
    color: $blue;
    display: flex;
    text-align: right;
    margin-left: 5px;
    @include textos;
  }
  .frame-9 {
    margin-top: 33px;
    width: 55px;
    height: 624px;
    margin-right: 80px;
  }
  .flex-wrapper-two {
    padding: 198px 0 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
  }
  .he-estudiado-2-grados-superiores-desarol {
    height: 151px;
    width: 726px;
    color: $blue;
    display: flex;
    margin-bottom: 147px;
    @include textos;
  }
  .me-considero-programador-full-stack-ya-qu {
    height: 200px;
    width: 726px;
    color: $blue;
    display: flex;
    margin-left: 30px;
    @include textos;
  }
  .frame-1 {
    background-color: $green;
   
    padding: 21px 51px;
    display: flex;
    align-items: flex-start;
  }
  .video-interactivo {
    max-width: 246px;
    color: rgba(0, 0, 0, 1);
    text-align: center;
    @include inter-40-black;
  }
  .si-deseas-saber-mas-mira-mi-video-intera {
    height: 100px;
    width: 714px;
    color: $blue;
    display: flex;
    align-items: center;
    text-align: center;
    
    @include inter-36-light;
  }
  </style>