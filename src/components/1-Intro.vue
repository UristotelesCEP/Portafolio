<template>
  <div class="PorfilePhoto">
          <img class="imagen" src="https://uristotelescep.github.io/media/photo2.png" alt="">
        </div>
    <div class="intro">
      <div class="relative-wrapper-one">
        <p class="hello-im-oriol-multiplatform-web-deve">
          <strong
            class="hello-im-oriol-multiplatform-web-deve-emphasis-0"
            >hello </strong
          > <br> I’m
          <strong
            class="hello-im-oriol-multiplatform-web-deve-emphasis-2"
            >Oriol<br /> </strong
          >Multiplatform &amp; Web Developer<br />
        </p>
        <div class="frame-1">
          <a  style="color: black;" href="https://www.linkedin.com/in/oriol-antr%C3%A0s-agut-a21b1a27/"><div class="hire-me">Hire Me</div></a> 
        </div>
        
        <img
          alt=""
          class="logo"
          src="https://static.overlay-tech.com/assets/1eb20c0d-0c9d-4bb9-ac34-bbc511db8fe8.svg"
        />
      </div>
      <div class="fondo-azul"></div>
    </div>
  </template>
  
  <script>
  export default {
    name: "Intro-com"
  };
  </script>
  
  <style lang="scss" scoped>
  @import "/src/Estilos.scss";
  .intro {
    background-color: rgba(255, 255, 255, 1);
    padding: 0 0 0 229px;
    display: flex;
    align-items: flex-start;
  }
  .relative-wrapper-one {
    margin-top: 254px;
    margin-right: 265px;
    position: relative;
  }
  .hello-im-oriol-multiplatform-web-deve {
    height: 200px;
    width: 786px;
    // display: flex;
    position: absolute;
    right: -100px;
    top: -52px;
    color: $blue;
    @include inter-40-black;
  }
  .hello-im-oriol-multiplatform-web-deve-emphasis-0 {
    color: $blue;
    @include inter-40-regular;
  }
  .hello-im-oriol-multiplatform-web-deve-emphasis-2 {
    color: $green;
    @include inter-64-black;
  }
  .frame-1 {
    background-color: $green;
    padding: 21px 51px;
    display: flex;
    align-items: flex-start;
    position: absolute;
    left: -24px;
    top: 212px;
    z-index: 9;
  }
  .PorfilePhoto {
    
    padding: 21px 51px;
    display: flex;
    align-items: flex-start;
    position: absolute;
    right: -44px;
    top: 62px;
  }
  .imagen
  {
    height: 941px;
    width: 990px;
  }
  .hire-me {
    color: rgba(0, 0, 0, 1);
    @include inter-40-black;
  }
  .logo {
    width: 657px;
    height: 593.51px;
    position: relative;
  }

  .fondo-azul {
    width: 100%;
    height: 907px;
    background-color: $blue;
  }
  </style>