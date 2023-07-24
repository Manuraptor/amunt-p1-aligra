<script>
    import { fade } from 'svelte/transition';
    import '/src/global.css'
    import imgprueba from '$lib/imagenes/AligraQueEs/repte-urba_regeneracio_aligra-1280x1524.jpg'
    import ArticleQueEsAligra from "$lib/componentes/ArticleQueEsAligra.svelte";
</script>
<div class="container">
    <div class="cards-container">
        <ArticleQueEsAligra>
            <h2>Regeneració Innovadora i Sostenible</h2>
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
    </div>
</div>

<style>
    .container {
        display: flex;
        align-items: flex-start;
    }

    .cards-container {
        flex: 1;
        margin-right: 70px;
    }

    .image-container {
        flex: 1;
        display: flex;
        justify-content: flex-end;

    }

    .image-container img {
        max-width: 100%;
        height: auto;
        margin-left: 20px;
        filter: grayscale(90%);
        transition: all 0.5s ease;
        cursor:pointer;
    }

    .image-container img:hover {
        transform: scale(1.1);
        filter: none;

    }



 /*  .container {
       display: flex;
       justify-content: space-between;
       align-items: flex-start;
   }

   .cards-container {
       width: 50%;
       display: flex;
       flex-wrap: wrap;
       margin-left: 50px;
       margin-top: 90px;

   }

   .card {
       flex: 0 0 100%;
       background-color: #f5f5f5;
       border-radius: 10px;
       padding: 30px;
       box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
       margin-bottom: 30px;
   }
   p{
       margin-top: 15px;
       letter-spacing: 1px;
   }

   .image-container {
       width: 40%;
       margin-left: 40px;
       object-fit: cover;
       filter: grayscale(90%);
       transition: all 0.5s ease;
       cursor:pointer;

   }
   .image-container:hover{
       transform: scale(1.1);
       filter: none;

   }

   img {
       width: 100%;
       height: auto;
       border-radius: 10px;
   }*/
</style>
