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
     <a href="https://straddle3.net/es/"><Componente imagen="{straddle3}" titulo="Straddle3:" texto= " Colꞏlectiu de Barcelona que treballa en arquitectura
                                i ciutat des d'una perspectiva crítica i inclusiva.

                                Ha desenvolupat projectes d'habitatge social, processos participatius,
                                intervencions en espais públics i recerca en la  construcció a  partir de
                                materials reutilitzats i reciclats."/></a>
    <a href="https://societatorganica.com/"><Componente imagen="{societatorganica}" titulo="Societat Orgànica:" texto
=" Sostenibilitat i ecologia aplicada a l’edificació. Cooperativa d’arquitectes que treballa en el paradigma de la sostenibilitat en el sector de l’edificació. La consideració del tancament del cicle dels materials com
a condició necessària per a aconseguir la sostenibilitat és el seu referent d’actuació."/></a>


    <a href="https://tejido.io/es/"> <Componente imagen="{tejido}" titulo="Tejido:" texto="Tejido: tecnologies de la informació aplicades a la ciutat.
            Cooperativa andalusa de base tecnològica que treballa en els àmbits de les tecnologies
            de codi obert per a la transformació urbana i social, l'arquitectura i l'art"/></a>

    <a href="https://aiguasol.coop/"><Componente  imagen="{aiguasol}" titulo="Aiguasol:"texto="Aiguasol: Enginyeria en instalꞏlacions sostenibles.
Cooperativa autogestionada que ofereix serveis d'enginyeria i consultoria en energia i aire.
A través d'una estructura horitzontal i socialment responsable, promou solucions innovadores
 per a reduir la petjada energètica i millorar la qualitat ambiental dels nostres entorns."/></a>

    <a href="https://www.tallfusta.com/"> <Componente imagen="{tallfusta}" titulo="Tallfusta:" texto=" Prefabricació lleugera. Empresa amb una àmplia
experiència en el sector de la construcció amb fusta. Sistemes avançats en solucions estructurals
i construcció prefabricada amb aquest material."/></a>

    <section>
        <div>
            <h3>L’equip es complementa amb la colꞏlaboració permanent de:</h3>
        </div>
        <div>
            <p> - Holaluz: experts en producció i distribució d’energía verda.</p>

            <p> - SiS Consultoría Acústica.</p>

            <p> - Maviteck consultors.</p>

            <p> - Melanie Theodosopoulou. Arquitecta i paisatgista.</p>
    </div>
    </section>
    <article>

        <a href="https://www.holaluz.com/"><img transition:fade src="{holaluz}" alt="logo"/> </a>
     <a href="https://sisconsultoria.com/"><img transition:fade src="{sis}" alt="logo"/></a>
     <a href="https://www.mavitecindustrial.com/"><img transition:fade src="{mavitec}" alt="logo"/></a>




    </article>
</main>

<style>

    main {
       display:flex;
        width: 100%;
        flex-direction: column;
        gap: 60px;
    }

    section {
        display: flex;
    justify-content: center;
        flex-direction: column;
        align-items: center;
    }

    article {

       margin-top:70px;
        width: 1000px;
        margin-bottom:25px;
        display: flex;
        flex-direction: row;
        justify-content: space-between

    }

    img {
        width: 150px;
        filter: grayscale(100%);
        transition: all 0.5s ease;
    }
    img:hover {
        filter: none;
        transform: scale(1.1);


    }




    a{
        text-decoration: none;
        color: black;
        font-size: 16px;
    }




</style>