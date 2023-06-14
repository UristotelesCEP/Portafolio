<template>
    <div class="manual-de-indetidad">
        <p class="manual-de-identidad">Manual De Identidad</p>
        <div class="content">
            <div class="frame-4">
                <p class="logotipo">Logotipo</p>
                <p class="descripcionLogo">
                    El logotipo de mi marca es una representación visual
                    de mis valores y personalidad. Está compuesto por un
                    triángulo que simboliza tanto la estabilidad y
                    equilibrio como el crecimiento y progreso constantes
                    que busco. El uso de los colores corporativos,
                    #34495E y #41B883, refuerza la sensación de
                    confianza, seriedad, vitalidad y energía positiva
                    que quiero transmitir.
                </p>
                <div class="logo">
                    <div class="frame-23">
                        <img alt="" src="https://static.overlay-tech.com/assets/4eee9806-7473-44b7-8ca5-e8c4bcad89dc.svg" />
                        <p class="uristoteles">Uristóteles</p>
                    </div>
                </div>
            </div>
            <div class="frame-5">
                <p class="paleta-colores">Paleta Colores</p>
                <p class="mi-paleta-de-colores-se-compone-principa">
                    Mi paleta de colores se compone principalmente de
                    dos tonos clave. El azul oscuro #34495E refleja
                    estabilidad y seriedad, representando mi firmeza en
                    ofrecer soluciones confiables y profesionales a mis
                    clientes. Por otro lado, el verde vibrante #41B883
                    evoca vitalidad, naturaleza y crecimiento, lo que
                    refleja el enfoque en la innovación constante y la
                    búsqueda de nuevas oportunidades.
                </p>
                <div class="colores">
                    <div>
                        <div class="frame-2">
                            <p class="num-34495e">#34495E</p>
                            <p class="cmyk-45-22-0-63">
                                CMYK(45%, 22%, 0%, 63%)
                            </p>
                        </div>


                    </div>

                    <div class="frame-3">
                        <p class="num-34495e">#41B883</p>
                        <p class="cmyk-65-0-29-28">
                            CMYK(65%, 0%, 29%, 28%)
                        </p>
                    </div>
                </div>
            </div>
            <div class="frame-6">
                <div class="flex-wrapper-one">
                    <p class="tipografia">Tipografia</p>
                    <p class="he-seleccionado-la-tipografia-jura-como">
                        He seleccionado la tipografía Jura como mi fuente
                        principal. Jura es una tipografía sans-serif
                        moderna y versátil, diseñada específicamente para
                        su uso en pantallas y dispositivos digitales. Su
                        diseño limpio y equilibrado asegura una excelente
                        legibilidad tanto en tamaños pequeños como
                        grandes. La elegancia y claridad de la tipografía
                        Jura refuerzan la imagen sofisticada y clara como
                        marca.
                    </p>
                </div>
                <p class="inter-inter-inter-inter-inter-inter-inte">
                    Inter<br />
                    <strong class="inter-inter-inter-inter-inter-inter-inte-emphasis-1">Inter<br /> </strong><strong
                        class="inter-inter-inter-inter-inter-inter-inte-emphasis-2">Inter<br /> </strong><strong
                        class="inter-inter-inter-inter-inter-inter-inte-emphasis-3">Inter<br /> </strong><strong
                        class="inter-inter-inter-inter-inter-inter-inte-emphasis-4">Inter<br /> </strong><strong
                        class="inter-inter-inter-inter-inter-inter-inte-emphasis-5">Inter<br /> </strong><strong
                        class="inter-inter-inter-inter-inter-inter-inte-emphasis-6">Inter<br /> </strong><strong
                        class="inter-inter-inter-inter-inter-inter-inte-emphasis-7">Inter</strong>
                </p>
            </div>
            <div class="frame-11">
                <div class="flex-wrapper-two">
                    <p class="voz-de-la-marca">Voz de la marca</p>
                    <p class="me-caracterizo-por-ser-una-persona-profe">
                        Me caracterizo por ser una persona profesional en
                        mi enfoque y comunicación. Utilizo un lenguaje
                        claro y preciso para transmitir mi experiencia y
                        confiabilidad. Busco establecer conexiones con las
                        personas, fomentando una actitud positiva y
                        motivadora en todas mis interacciones.
                    </p>
                </div>
                <div class="speaker-svgrepo-com-1">
                    <img alt="" class="group-two"
                        src="https://static.overlay-tech.com/assets/450aa918-5e61-41eb-bde0-04b7388d8603.svg" />
                </div>
            </div>


        </div>
    </div>
</template>
  
<script>
export default {
    name: "ManualDeIndetidad"
};
</script>
  
<style lang="scss" scoped>
@import "/src/Estilos.scss";

.manual-de-indetidad {
    background-color: rgba(255, 255, 255, 1);
    padding: 27px 61px;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.manual-de-identidad {
    color: $blue;
    margin-bottom: 91px;
    @include inter-64-extra-light;
}
.content
{
    display: flex;
    flex-direction: column;
    align-items: baseline;
}
.frame-4 {
    margin-bottom: 91px;
    padding: 0 527px 97px 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    height: 341px;
    width: 1241px;
    position: relative;
}

.logotipo {
    font-family: "Inter";
    font-size: 48px;
    font-weight: 700;
    line-height: normal;
    color: $blue;
    margin-bottom: 19px;
}

.descripcionLogo {
    max-width: 1241px;
    color: $blue;
    @include textos;
}

.logo {
    padding: 0 19.14px 16.99px 18.91px;
    display: flex;
    align-items: flex-start;
    position: absolute;
    right: 0;
    top: 28px;
}

.frame-23 {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.uristoteles {
    height: 24.37%;
    font-family: "Jura";
    font-size: 48px;
    font-weight: 500;
    line-height: normal;
    color: $blue;
    align-self: stretch;

    text-align: center;
}

.frame-5 {
    margin-bottom: 91px;
    padding: 29px 96px 25px 0;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    height: 720px;
    width: 1679px;
}

.paleta-colores {
    font-family: "Inter";
    font-size: 48px;
    font-weight: 700;
    line-height: normal;
    color: $green;
    margin-bottom: 46px;
}

.mi-paleta-de-colores-se-compone-principa {
    max-width: 1679px;
    color: $blue;
    margin-bottom: 5px;
    @include textos;
}

.colores {
    background-color: rgba(254, 254, 254, 1);
    margin-left: 166px;
    overflow: hidden;
    border-radius: 20px;
    padding: 15px 169px 91px;
    display: flex;
    align-items: flex-start;
    justify-content: center;
}

.frame-2 {
    background-color: $blue;
    margin-right: 535px;
    border-radius: 50%;
    padding: 118px 56px 119px 48px;
    width: 181px;
    height: 48px;
    display: flex;
    flex-direction: column;
    position: relative;
}

.num-34495e {
    font-family: "Inter";
    font-size: 40px;
    font-weight: 600;
    line-height: normal;
    margin: auto;
    color: rgba(255, 255, 255, 1);
}

.cmyk-45-22-0-63 {
    color: rgba(255, 255, 255, 1);
    font-size: small;
    margin: auto;
    font-family: "Inter";

}

.frame-3 {
    background-color: $green;
    border-radius: 50%;
    padding: 118px 54px 119px 55px;
    width: 176px;
    height: 48px;
    display: flex;
    flex-direction: column;
    position: relative;
}

.cmyk-65-0-29-28 {
    color: rgba(255, 255, 255, 1);
    font-size: small;
    margin: auto;
    font-family: "Inter";
}

.frame-6 {
    margin-bottom: 91px;
    padding: 34px 182px 0 0;
    display: flex;
    align-items: flex-start;
    height: 384px;
    width: 1578px;
}

.flex-wrapper-one {
    margin-right: 251px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.tipografia {
    font-family: "Inter";
    font-size: 48px;
    font-weight: 700;
    line-height: normal;
    color: $blue;
    margin-bottom: 39px;
}

.he-seleccionado-la-tipografia-jura-como {
    max-width: 1231px;
    color: $blue;
    @include textos;
}

.inter-inter-inter-inter-inter-inter-inte {
    text-align: center;
    font-family: "Inter";
    font-size: 40px;
    font-weight: 100;
    line-height: normal;
    color: rgba(0, 0, 0, 1);
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-1 {
    font-family: "Inter";
    font-size: 40px;
    font-weight: 200;
    line-height: normal;
    color: rgba(0, 0, 0, 1);
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-2 {
    color: rgba(0, 0, 0, 1);
    @include inter-40-regular;
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-3 {
    font-family: "Inter";
    font-size: 40px;
    font-weight: 500;
    line-height: normal;
    color: rgba(0, 0, 0, 1);
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-4 {
    font-family: "Inter";
    font-size: 40px;
    font-weight: 600;
    line-height: normal;
    color: rgba(0, 0, 0, 1);
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-5 {
    font-family: "Inter";
    font-size: 40px;
    font-weight: 700;
    line-height: normal;
    color: rgba(0, 0, 0, 1);
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-6 {
    font-family: "Inter";
    font-size: 40px;
    font-weight: 800;
    line-height: normal;
    color: rgba(0, 0, 0, 1);
}

.inter-inter-inter-inter-inter-inter-inte-emphasis-7 {
    color: rgba(0, 0, 0, 1);
    @include inter-40-black;
}

.frame-11 {
    display: flex;
    align-items: flex-start;
    height: auto;
    width: 1718px;
}

.flex-wrapper-two {
    margin-right: 111px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
}

.voz-de-la-marca {
    font-family: "Inter";
    font-size: 48px;
    font-weight: 700;
    line-height: normal;
    color: $green;
    margin-bottom: 37px;
}

.me-caracterizo-por-ser-una-persona-profe {
    height: 186px;
    width: 1326px;
    color: $blue;
    display: flex;
    @include textos;
}

.speaker-svgrepo-com-1 {
    padding: 6.04px 6.05px 6.06px 6.04px;
    display: flex;
    margin: auto;
    align-items: center;
}

.group-two {
    width: 268.91px;
    height: 268.9px;
}
</style>