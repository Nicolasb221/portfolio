<template>
    <header class="container-h">
        <div class="container__name">
            <a href="/"><span class="letra">N</span><span class="letra">i</span><span class="letra">c</span><span class="letra">o</span><span class="letra">l</span><span class="letra">á</span><span class="letra">s</span></a>
        </div>
        <ul class="container__list">
            <li @click="inicio" :class="liActive[0]"><fa :icon="['fas', 'house']" class="container__list-i"/>Inicio</li>
            <li @click="formacion" :class="liActive[1]" > <fa :icon="['fas', 'brain']" class="container__list-i"/>Formación</li>
            <li @click="proyectos" :class="liActive[2]" > <fa :icon="['fas', 'check-double']" class="container__list-i" />Proyectos</li>
        </ul>
    </header>
</template>

<script setup>
import { ref, inject} from 'vue';
const flagInicio = inject('flagInicio', ref(false));
const flagFormacion = inject('flagFormacion', ref(false));
const flagProyectos = inject('flagProyectos', ref(false));
const liActive = ref(['li-active','li-disable','li-disable','li-disable'])



const inicio = () => {
    flagInicio.value = true;
    flagFormacion.value = false;
    flagProyectos.value = false;
    liActive.value = ['li-active','li-disable','li-disable','li-disable']
};

const formacion = () => {
    flagInicio.value = false;
    flagFormacion.value = true;
    flagProyectos.value = false;
    liActive.value = ['li-disable','li-active','li-disable','li-disable']

}
const proyectos = () => {
    flagInicio.value = false;
    flagFormacion.value = false;
    flagProyectos.value = true;
    liActive.value = ['li-disable','li-disable','li-active','li-disable']

}


</script>

<style scoped>
    .container-h{
        display: flex;
        position: relative;
        width: 100%;
        height: 20px;
        justify-content: space-between;
        background-color: var(--color-header-n);
        padding: 10px 0;
        filter: drop-shadow(0 0 20px #000000);
        z-index: 10000;
        
    }
    .container__name{
        margin: 5px 30px 5px 30px;
        font-family:'Press Start 2P', sans-serif;
        font-size: 15px;
        cursor: pointer;
        
    }
    .container__list{
        display: flex;
        gap: 30px;
        list-style: none;
        padding: 0;
        margin: 0 30px 0 0;
        align-items: center;
        font-size: 14px;
    }
    li{
        cursor: pointer;
        display: flex;
        margin: 5px;

    }
    li:hover{
        color: var(--color-header-name-n);
        transition: color .5s ease-in-out;
    }
    .container__list-i{
        display: flex;
        justify-content: center;
        margin: 0 10px 10px 0;
    }
    .li-active{
        color: var(--color-header-name-n);
        scale: 1.2;
        border-bottom: 2px solid var(--color-header-name-n);
        transition: all 2s ease-in-out;
    
    }
    .li-disable{
        color: #fff;
        transition: all 1s ease-in-out;
    }
    .letra {
      display: inline-block;
      padding-right: 10px;
      transform: scale(1);
      transition: transform 0.3s ease-in-out;
      animation: scaleUp 1.4s infinite alternate;
    }

    @keyframes scaleUp {
      from {
        transform: scale(1);
        color: #9ec4bb;
      }
      to {
        transform: scale(1.5);
        color: var(--color-header-name-n);
        opacity: .6;
      }
    }

    /* Aplicar un retraso a cada letra */
    .letra:nth-child(1) { animation-delay: 0s; }
    .letra:nth-child(2) { animation-delay: 0.2s; }
    .letra:nth-child(3) { animation-delay: 0.4s; }
    .letra:nth-child(4) { animation-delay: 0.6s; }
    .letra:nth-child(5) { animation-delay: 0.8s; }
    .letra:nth-child(6) { animation-delay: 1s; }
    .letra:nth-child(7) { animation-delay: 1.2s; }
    @media (max-width: 650px) {
    .container__name{
        font-size: 10px; 
        margin: 5px 10px 5px 10px;

    }
    .letra {
      padding-right: 5px;
    }
    .container__list{
        gap: 10px;
        margin: 0 10px 0 0;
        font-size: 9px;
    }
    }

</style>