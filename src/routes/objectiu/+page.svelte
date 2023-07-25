<script>
    import { fade } from 'svelte/transition';
    import '/src/global.css'
    import imgprueba from '$lib/imagenes/AligraQueEs/repte-urba_regeneracio_aligra-1280x1524.jpg'
    import ArticleQueEsAligra from "$lib/componentes/ArticleQueEsAligra.svelte";
</script>

<main>
<div class="container">
    <div class="cards-container">
        <ArticleQueEsAligra>
            <h2>Regeneració Innovadora Sostenible</h2>
            <p>Aligra es un proyecto ganador de la convocatoria para la "Regeneració d’edificis d’habitatges amb sistemes innovadors sostenibles" de la fundació BitHàbitat. El Ayuntamiento de Barcelona busca soluciones integrales para mejorar la habitabilidad y el rendimiento energético de los edificios de la ciudad.</p>

        </ArticleQueEsAligra>
        <ArticleQueEsAligra>
            <h2>Millora Energètica i Sostenibilitat en Edificis de Barcelona</h2>
            <p>El objetivo del proyecto Aligra es mejorar el rendimiento energético de los edificios de Barcelona mediante el uso de nuevos materiales, tecnologías y diseños innovadores. También se busca abordar aspectos como el uso eficiente de los recursos, la mitigación del cambio climático y la resiliencia.</p>

        </ArticleQueEsAligra>



        <ArticleQueEsAligra>
            <h2>Una Solució Flexible i Sostenible per al Repte Urbà</h2>
            <p> El sistema Aligra responde de manera rigurosa y flexible al Repte Urbà. Se basa en una solución multicapa y escalable, desarrollada en colaboración con diversas empresas, que aprovecha la experiencia acumulada en el diseño arquitectónico ecológico. El sistema es genérico, de código abierto y adaptable a diferentes situaciones constructivas, sin las restricciones impuestas por patentes privativas.</p>

        </ArticleQueEsAligra>

        <ArticleQueEsAligra>
            <h2> Adaptabilitat i Variedat en la Transformació Urbana i Arquitectònica</h2>
            <p>Aligra está concebido para adaptarse a una amplia variedad de situaciones arquitectónicas y urbanas. Se han analizado diversas configuraciones, desde edificios residenciales hasta edificios menos habituales no alineados a la calle.<br> Se han considerado ampliaciones de espacio privado, introducción de galerías, generación de espacios abiertos privados y colectivos, así como la posibilidad de incluir nuevos núcleos de comunicación vertical.<br> Además, se propone un sistema en el que las capas de acabado son intercambiables para ofrecer diversidad de texturas y colores en la fachada.</p>

        </ArticleQueEsAligra>


    </div>

    <div class="image-container">
        <img transition:fade src={imgprueba} alt="">
        <img transition:fade src={imgprueba} alt="">

    </div>

</div>
</main>

<style>

 .container {
        display: flex;
        align-items: flex-start;
    }

   .cards-container {
        flex: 1;
        margin-left: -100px;
        margin-right: 100px;
    }

    .image-container {
        flex: 1;
        display: flex;
       justify-content: flex-end;
        margin-right: -220px;
        flex-direction: column;
        position: relative;
        gap:30px;
        margin-top: 430px;


    }

    .image-container {
        max-width: 400px;
        height: 600px;
        margin-left: 20px;
        filter: grayscale(100%);
        transition: all 0.5s ease;
        cursor:pointer;
    }

    .image-container:hover {
        transform: scale(1.1);
        filter: none;

    }









</style>

