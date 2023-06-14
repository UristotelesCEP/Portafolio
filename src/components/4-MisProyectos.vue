<template>
    <div class="mis-proyectos">
      <p class="proyectos-recientes">Proyectos recientes</p>
      <div class="flex-wrapper-one">
        <div class="rectangle-3"></div>
        <div class="rectangle-3"></div>
        <div class="rectangle-3"></div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: "MisProyectos"
  };
  </script>
  
  <style lang="scss" scoped>
  @import "/src/Estilos.scss";
  .mis-proyectos {
    background-color: rgba(255, 255, 255, 1);
    padding: 91px 105px 151px 104px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  
  .flex-wrapper-one {
    display: flex;
    justify-content: center;
    margin-top: 36px;
  }
  
  .proyectos-recientes {
    color: $blue;
    margin-bottom: 24px;
    @include inter-64-extra-light;
  }
  
  .rectangle-3 {
    width: 518px;
    height: 518px;
    background-color: rgba(217, 217, 217, 1);
    margin: 0 18px;
  }
  </style>
  