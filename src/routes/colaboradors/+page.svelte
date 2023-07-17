<script>
    import '/src/global.css'
    import { fade } from 'svelte/transition';

    import Componente from "$lib/componentes/Componente.svelte";
    import straddle3 from "$lib/imagenes/Colaboradors/image 1.png";
    import societatorganica from "$lib/imagenes/Colaboradors/image 2.png";
    import tejido from "$lib/imagenes/Colaboradors/image 17.png";
    import aiguasol from "$lib/imagenes/Colaboradors/image 3.png";
    import tallfusta from "$lib/imagenes/Colaboradors/image 18.png";
    import holaluz from "$lib/imagenes/Colaboradors/image41.png";
    import sis from "$lib/imagenes/Colaboradors/image 5.png";
    import mavitec from "$lib/imagenes/Colaboradors/image 19.png";


</script>

<main>
    <Componente imagen="{straddle3}" texto=" Straddle3:  Colꞏlectiu de Barcelona que treballa en arquitectura
                                i ciutat des d'una perspectiva crítica i inclusiva.

                                Ha desenvolupat projectes d'habitatge social, processos participatius,
                                intervencions en espais públics i recerca en la  construcció a  partir de
                                materials reutilitzats i reciclats."/>


    <Componente imagen="{societatorganica}" texto="Societat Orgànica:   Sostenibilitat i ecologia aplicada a l’edificació. Cooperativa d’arquitectes que treballa en el paradigma de la sostenibilitat en el sector de l’edificació. La consideració del tancament del cicle dels materials com
a condició necessària per a aconseguir la sostenibilitat és el seu referent d’actuació."/>


    <Componente imagen="{tejido}" texto="Tejido: tecnologies de la informació aplicades a la ciutat.
            Cooperativa andalusa de base tecnològica que treballa en els àmbits de les tecnologies
            de codi obert per a la transformació urbana i social, l'arquitectura i l'art"/>

    <Componente imagen="{aiguasol}" texto="Aiguasol: Enginyeria en instalꞏlacions sostenibles.
Cooperativa autogestionada que ofereix serveis d'enginyeria i consultoria en energia i aire.
A través d'una estructura horitzontal i socialment responsable, promou solucions innovadores
 per a reduir la petjada energètica i millorar la qualitat ambiental dels nostres entorns."/>

    <Componente imagen="{tallfusta}" texto="Tallfusta: Prefabricació lleugera. Empresa amb una àmplia
experiència en el sector de la construcció amb fusta. Sistemes avançats en solucions estructurals
i construcció prefabricada amb aquest material."/>

    <div>
        <p>L’equip es complementa amb la colꞏlaboració permanent de:<br><br></p>
        <ul>
            <p> - Holaluz: experts en producció i distribució d’energía verda.<br><br></p>

            <p> - SiS Consultoría Acústica.<br><br></p>

            <p> - Maviteck consultors.<br><br></p>

            <p> - Melanie Theodosopoulou. Arquitecta i paisatgista.<br><br></p>
        </ul>
    </div>

    <article>

        <img transition:fade src="{holaluz}" alt="logo"/>;
        <img transition:fade src="{sis}" alt="logo"/>;
        <img transition:fade src="{mavitec}" alt="logo"/>;


    </article>
</main>

<style>

    main {
        width: 100%;
        padding-top: 225px;
    }

    div {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
    }

    article {
        margin-top:40px;
        margin-left: 280px;
        width: 1000px;
        margin-bottom:60px;
        display: flex;
        flex-direction: row;
        justify-content: space-between

    }

    img {
        width: 200px;
        filter: grayscale(75%);
        transition: all 0.5s ease;
    }
    img:hover {
        filter: none;
    }

</style>