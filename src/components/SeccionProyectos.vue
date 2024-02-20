<template>
    <section class="container">
        <section class="container__proyectos">
            <article :class="classname[0]" @click="focuscn1">
                <div class="tb" v-show="classname[0]=='container-active'">
                    <div class="container-link" >
                        <a href="https://topotronv2.netlify.app/" target="_blank" :style="[colorLink, estiloColor, '--fa-animation-duration: 4s']" ><fa :icon="['fas', 'link']" size="1x" class="sombra" shake/></a>
                    </div>
                    <p :style="estiloColor">TopoTron es un juego de golpear al topo, fue creado con la finalidad de afianzar y poner en práctica mis conocimientos en HTML, CSS y JavaScript nativos, mejoré su logica de programación implementando jQuery.</p>
                    <div class="container-tb">
                        <h1 class="titulo" :style="estiloColor">TopoTron</h1>
                        <div class="container-tb-icos">
                            <fa :icon="['fab', 'html5']" style="color: #E9532D; --fa-animation-duration: 1s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'css3-alt']" style="color: #036FBA; --fa-animation-duration: 2s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'square-js']"  style="color: #F7E018; --fa-animation-duration: 3s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                        </div>
                    </div>
                </div>
                <div div class="tbd" v-show="classname[0]=='container__profile-proyecto'">
                    <fa :icon="['fas', 'atom']" spin size="3x" style="color: #D5A86A; --fa-animation-duration: 3s" class="fa"/>
                </div>
                <img class="background" src="../assets/topotronim.png" alt="TopoTron">
            </article>
            <article :class="classname[1]" @click="focuscn2">
                <div class="tb" v-show="classname[1]=='container-active'">
                    <div class="container-link" >
                        <a href="https://infinitytimer.netlify.app/" target="_blank" :style="[colorLink, estiloColor, '--fa-animation-duration: 4s']"><fa :icon="['fas', 'link']" size="1x" class="sombra" shake/></a>
                    </div>
                    <p :style="estiloColor">InfinityTimer, es un proyecto creado para poner en práctica mis conocimientos en HTML CSS y JavaScript nativo.</p>
                    <div class="container-tb">
                        <h1 class="titulo" :style="estiloColor">InfinityTimer</h1>
                        <div class="container-tb-icos">
                            <fa :icon="['fab', 'html5']" style="color: #E9532D; --fa-animation-duration: 1s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'css3-alt']" style="color: #036FBA; --fa-animation-duration: 2s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'square-js']"  style="color: #F7E018; --fa-animation-duration: 3s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                        </div>
                    </div>
                </div>
                <div div class="tbd" v-show="classname[1]=='container__profile-proyecto'">
                    <fa :icon="['fas', 'atom']" spin size="3x" style="color: #5F3362; --fa-animation-duration: 3s" class="fa"/>
                </div>
                <img class="background" src="../assets/infinityim.png" alt="InfinityTimer">
            </article>
            <article :class="classname[2]" @click="focuscn3">
                <div class="tb" v-show="classname[2]=='container-active'">
                    <div class="container-link" >
                        <a href="https://busquegithub.netlify.app/" target="_blank" :style="[colorLink, estiloColor, '--fa-animation-duration: 4s']"><fa :icon="['fas', 'link']" size="1x" class="sombra" shake/></a>
                    </div>
                    <p :style="estiloColor">En este proyecto utilicé el framework Vue.js, además puse a prueba mis conocimientos en el manejo de APIs y localStorage del navegador.</p>
                    <div class="container-tb">
                        <h1 class="titulo" :style="estiloColor">Buscador de usuarios github</h1>
                        <div class="container-tb-icos">
                            <fa :icon="['fab', 'html5']" style="color: #E9532D; --fa-animation-duration: .9s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'css3-alt']" style="color: #036FBA; --fa-animation-duration: 2s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'square-js']"  style="color: #F7E018; --fa-animation-duration: 1.9s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'vuejs']" style="color: #41B883;--fa-animation-duration: 1s;--fa-beat-fade-scale: 1.1;" size="2x" class="sombra" beat-fade/>
                        </div>
                    </div>
                </div>
                <div div class="tbd" v-show="classname[2]=='container__profile-proyecto'">
                    <fa :icon="['fas', 'atom']" spin-pulse size="3x" style="color: #A7B15D; --fa-animation-duration: 1.5s" class="fa"/>
                </div>
                <img class="background" src="../assets/bughim.png" alt="BusquedaGitHub">
            </article>
            <article :class="classname[3]" @click="focuscn4">
                <div class="tb" v-show="classname[3]=='container-active'">
                    <div class="container-link" >
                        <a href="https://listaprofesores.netlify.app/" target="_blank" :style="[colorLink, estiloColor, '--fa-animation-duration: 4s'] "><fa :icon="['fas', 'link']" size="1x" class="sombra" shake/></a>
                    </div>
                    <p :style="estiloColor">Formulario para añadir profesores creado con vue3, responsive, funcionalidad de añadir y quitar materias, asi como añadir y eliminar profesores.</p>
                    <div class="container-tb">
                        <h1 class="titulo" :style="estiloColor">Formulario Profesores</h1>
                        <div class="container-tb-icos">
                            <fa :icon="['fab', 'html5']" style="color: #E9532D; --fa-animation-duration: .9s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'css3-alt']" style="color: #036FBA; --fa-animation-duration: 2s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'square-js']"  style="color: #F7E018; --fa-animation-duration: 1.9s;--fa-beat-fade-scale: 1.1; " size="2x" class="sombra" beat-fade/>
                            <fa :icon="['fab', 'vuejs']" style="color: #41B883;--fa-animation-duration: 1s;--fa-beat-fade-scale: 1.1;" size="2x" class="sombra" beat-fade/>
                        </div>
                    </div>
                </div>
                <div div class="tbd" v-show="classname[3]=='container__profile-proyecto'">
                    <fa :icon="['fas', 'atom']" spin spin-reverse size="3x" style="color: #A2B283; --fa-animation-duration: 3s" class="fa"/>
                </div>
                <img class="background" src="../assets/fpim.png" alt="FormularioProfesores">
            </article>
            <article :class="classname[4]" @click="focuscn5">
                <div class="tb" v-show="classname[4]=='container-active'">
                    <div class="container-link" >
                        <a href="https://github.com/Nicolasb221/BCI-Drone-Control" target="_blank" :style="[colorLink, estiloColor, '--fa-animation-duration: 4s'] "><fa :icon="['fas', 'link']" size="1x" class="sombra" shake/></a>
                    </div>
                    <p :style="estiloColor">Tesis de Pregrado, Ingeniería Electrónica. Realizada por: -Nicolás Enrique Rodríguez Villate -Nicolás Alberto Bravo Silva durante el año 2022, realizamos el manejo de un drone mediante el uso de señales de electroencefalografía (EEG) y electrooculografía (EOG)</p>
                    <div class="container-tb">
                        <h1 class="titulo" :style="estiloColor">BCI Drone Control</h1>
                        <div class="container-tb-icos">
                            <img class="ico-ml" src="../assets/Matlab_Logo.png" alt="matlabico">
                            <img class="ico-cs" src="../assets/CoppeliaSim.png" alt="coppeliasimico">
                        </div>
                    </div>
                </div>
                <div div class="tbd" v-show="classname[4]=='container__profile-proyecto'">
                    <fa :icon="['fas', 'atom']" spin spin-reverse size="3x" style="color: #FFDD19; --fa-animation-duration: 3s" class="fa"/>
                </div>
                <img class="background" src="../assets/bcidcim.jpg" alt="BCI">
            </article>
        </section>
    </section>
</template>

<script setup>
    import {ref} from 'vue';
    const classname = ref(['container-active','container__profile-proyecto','container__profile-proyecto','container__profile-proyecto','container__profile-proyecto']);
    const estiloColor = ref('filter: drop-shadow(5px 5px 5px #b48d00)');
    const colorLink = ref('color: #D5A86A');

    const focuscn1 = () =>{
        classname.value = ['container-active','container__profile-proyecto','container__profile-proyecto','container__profile-proyecto','container__profile-proyecto'];
        estiloColor.value = 'filter: drop-shadow(5px 5px 5px #b48d00)';
        colorLink.value = 'color: #D5A86A';
    }
    const focuscn2 = () =>{
        classname.value = ['container__profile-proyecto','container-active','container__profile-proyecto','container__profile-proyecto','container__profile-proyecto'];
        estiloColor.value = 'filter: drop-shadow(5px 5px 5px #98A0B1)';
        colorLink.value = 'color: #5A285A';

    }
    const focuscn3 = () =>{
        classname.value = ['container__profile-proyecto','container__profile-proyecto','container-active','container__profile-proyecto','container__profile-proyecto'];
        estiloColor.value = 'filter: drop-shadow(5px 5px 5px #A7B15D)';
        colorLink.value = 'color: #A7B15D';
    }
    const focuscn4 = () =>{
        classname.value = ['container__profile-proyecto','container__profile-proyecto','container__profile-proyecto','container-active','container__profile-proyecto'];
        estiloColor.value = 'filter: drop-shadow(5px 5px 5px #A2B283)';
        colorLink.value = 'color: #A2B283';
    }
    const focuscn5 = () =>{
        classname.value = ['container__profile-proyecto','container__profile-proyecto','container__profile-proyecto','container__profile-proyecto','container-active'];
        estiloColor.value = 'filter: drop-shadow(5px 5px 5px #FFDD19)';
        colorLink.value = 'color: #FFDD19';
    }
</script>

<style scoped>
    .container{
        align-items: center;
        filter: drop-shadow(0 0 50px #06b3f25b);
    }
    .container__proyectos{
        width: 95%;
        height: 95%;
        display: flex;
        gap: 20px;
        max-width: 1900px;
        padding: 50px;
        animation: despliegue 1s cubic-bezier(.28,1.05,.87,.19);
        box-sizing: border-box;
        border-radius: 40px;
        filter: drop-shadow(0 0 500px #06b3f25b);

    }
    .container__profile-proyecto{
        min-width: 100px;
        height: 100%;
        border-radius: 50px;
        overflow: hidden;
        display: flex;
        align-items: flex-end;
        cursor: pointer;
        position: relative;
        opacity: .5;
        transition: .7s cubic-bezier(0.455, 0.03, 0.515, 0.955);
        box-shadow: 0 0 15px #06b3f2;



    }
    .container__profile-proyecto:hover{
        opacity: 1;
        box-shadow: 0 0 55px #06b3f2;


    }
    .container-active{
        height: 100%;
        border-radius: 30px;
        overflow: hidden;
        display: flex;
        align-items: flex-end;
        position: relative;
        transition: .7s cubic-bezier(0.455, 0.03, 0.515, 0.955);
        flex-grow: 100;
        box-shadow: 0 0 15px #06b3f2;


    }
    img {
        width: 100%;
        height: 100%;
        display: block;
    }
    .container__profile-proyecto > .background {
        position: absolute;
        inset: 0;
        object-fit: cover;
        object-position: center;
        filter: brightness(0.8);
        border-radius: 30px;
    }
    .tb, .tbd{
        display: flex;
        flex-direction: column-reverse;
        height: 100%;
        width: 100%;
        position: absolute;
        z-index: 1000;
        border-image: fill 0 linear-gradient(#0001,#000);

    }
    .tbd{
        padding-bottom: 50px;
        border-image: fill 0 linear-gradient(#0001,#0000007e);
    }
    .fa{
        filter: opacity(1);
        z-index: 10000;
        filter: drop-shadow(5px 5px 20px #ffff70c8)
    }
    .tb > p{
        color: #fff;
        padding: 0 30px 0 30px;
        font-size: 25px;
        text-align: center;
    }
    .titulo{
        display: flex;
        flex-wrap: wrap;
        color: #fff;
        font-family:'Press Start 2P', sans-serif;
        font-size: 37px;
        margin: 20px;
    }
    .container-tb{
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        flex-direction: column;
        
    }
    .container-tb-icos{
        display: flex;
        align-items: center;
        gap: 10px;
        padding: 0 30px 0 30px;
        width: min-content;
    }
    .sombra{
        filter: drop-shadow(5px 5px 4px #000000);
    }
    .container-link{
        display: flex;
        padding: 0px 30px 30px 30px;
        justify-content: center;
        transition: 0.5s filter ease-in;
    }
    .container-link:hover{
        filter: drop-shadow(0px 0px 13px #7d7d7d);
        transition: 0.5s filter ease-in;
    }
    .ico-ml{
        width: 50px;
    }
    .ico-cs{
        width: 200px;
        filter: drop-shadow(0px 0px 3px #ffffff);
        
    }
    @keyframes despliegue {
    0% {
        width: 0%;
        filter:opacity(0);
    }
    50%{
        width: 25%;
        filter: opacity(.5);
    }
    100% {
        width: 90%;
        filter:opacity(1);
    }
    }
    @media (max-width: 1500px) {
        .container__profile-proyecto{
            min-width: 70px;
        }
    }  
    @media (max-width: 935px) {
        .container__proyectos{
            flex-direction: column;
            padding: 0;

        }
        .container__profile-proyecto{
        min-width: 100px;
        height: 90px;
        }
        .tbd{
            padding-bottom: 10px;
            display: flex;
            place-self: center;
        }
        .tb > p{
            font-size: 17px;
        }
        .titulo{
            font-size: 40px;
        }
        @keyframes despliegue {
            0% {
                height: 0%;
                filter:opacity(0);
            }
            50%{
                height: 25%;
                filter: opacity(.5);
            }
            100% {
                height: 90%;
                filter:opacity(1);
            }
        }
    } 
    @media (max-width: 500px) {
        .tb > p{
            font-size: 10px;
            padding: 0px 15px 5px 15px;

        }
        .container__proyectos{
            width: 90%;
            height: 95%;

        }
        
        .titulo{
            font-size: 20px;
            padding: 0px 15px 0px 15px;

        }
        .ico-ml{
            width: 20px;
        }
        .ico-cs{
            width: 150px;
            filter: drop-shadow(0px 0px 3px #ffffff);
            
        }
        .container-tb{
            gap: 0px;
        }
        .tbd{
            padding-bottom: 0;
        }
    } 
</style>