<template>
  <HeaderNav/>
  <SeccionPrincipal v-show="flagInicio"/>
  <SeccionHabilidades v-show="flagHabilidades"/>
  <SeccionFormacion v-show="flagFormacion"/>
  <SeccionProyectos v-show="flagProyectos"/>

</template>

<script setup>
import HeaderNav from './components/HeaderNav.vue';
import SeccionPrincipal from './components/SeccionPrincipal.vue';
import SeccionHabilidades from './components/SeccionHabilidades.vue';
import SeccionFormacion from './components/SeccionFormacion.vue';
import SeccionProyectos from './components/SeccionProyectos.vue';

import { ref, provide } from 'vue';

const flagInicio = ref(true); //true
const flagHabilidades = ref(false);
const flagFormacion = ref(false);
const flagProyectos = ref(false);


provide('flagInicio', flagInicio);
provide('flagHabilidades', flagHabilidades);
provide('flagFormacion', flagFormacion);
provide('flagProyectos', flagProyectos);


</script>

<style>
  :root{
    --color-fondo-n : linear-gradient(#3a3132f0,#181717);
    --color-desplegable-n : #05d4f833;
    --color-header-n: #252122;
    --color-header-name-n: #009ddd;
    --color-titulo-modal-n: #05d3f8;
  }
  body{
    margin: 0;
    background: var(--color-fondo-n);
    font-family: 'Chakra Petch', sans-serif;
    user-select: none;
    overflow: hidden;
    height: 100vh;
  }
  .container{
    width: 100%;
    height: 91vh;
    display: flex;
    justify-content: center;
  }
  .container__profile{
    width: 70%;
    height: 90%;
    border-radius: 0 0 30px 30px;
    background: var(--color-desplegable-n);
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    box-shadow: 0 0 40px #9ec4bb50;
    filter: drop-shadow(0 0 20px #9ec4bb);
    animation: despliegue 1.5s cubic-bezier(1,.03,.21,.76);
    gap: 30px;
    flex-wrap: nowrap;
    overflow: hidden;
    box-sizing: border-box;
    padding: 40px;
  }
  a:link, a:visited, a:active{
    text-decoration: none;
    color: white;
  }
    
  /* animaciones */

  @keyframes despliegue {0% {height: 0; opacity: 0;} 100% {height: 90%; opacity: 1;}}
  @keyframes typing {from {width: 50%;opacity: 0;}}
  @keyframes typing2 {from {width: 0;}}
  @keyframes blink {50% {border-color: transparent;}}
  @keyframes despliegue_text {0% {opacity: 0;}90%{opacity: 0;}100% {opacity: 1;}}
  @keyframes scaleupd {from{scale: 1; opacity: 1;}to{scale: 1.5; opacity: .5;}}


</style>
