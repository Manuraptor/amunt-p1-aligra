<script>
    import imgprueba from '$lib/imagenes/AligraQueEs/repte-urba_regeneracio_aligra-1280x1524.jpg'
</script>
<div class="container">
    <div class="cards-container">
        <div class="card">
            <h2>Idea principal 1</h2>
            <p>Aligra es un proyecto ganador de la convocatoria para la "Regeneració d’edificis d’habitatges amb sistemes innovadors sostenibles" de la fundació BitHàbitat. El Ayuntamiento de Barcelona busca soluciones integrales para mejorar la habitabilidad y el rendimiento energético de los edificios de la ciudad.</p>
        </div>

        <div class="card">
            <h2>Idea principal 2</h2>
            <p>El objetivo del proyecto Aligra es mejorar el rendimiento energético de los edificios de Barcelona mediante el uso de nuevos materiales, tecnologías y diseños innovadores. También se busca abordar aspectos como el uso eficiente de los recursos, la mitigación del cambio climático y la resiliencia.</p>
        </div>

        <div class="card">
            <h2>Idea principal 3</h2>
            <p> El sistema Aligra responde de manera rigurosa y flexible al Repte Urbà. Se basa en una solución multicapa y escalable, desarrollada en colaboración con diversas empresas, que aprovecha la experiencia acumulada en el diseño arquitectónico ecológico. El sistema es genérico, de código abierto y adaptable a diferentes situaciones constructivas, sin las restricciones impuestas por patentes privativas.</p>
        </div>

        <div class="card">
            <h2>Idea principal 4</h2>
            <p>Aligra está concebido para adaptarse a una amplia variedad de situaciones arquitectónicas y urbanas. Se han analizado diversas configuraciones, desde edificios residenciales hasta edificios menos habituales no alineados a la calle. Se han considerado ampliaciones de espacio privado, introducción de galerías, generación de espacios abiertos privados y colectivos, así como la posibilidad de incluir nuevos núcleos de comunicación vertical. Además, se propone un sistema en el que las capas de acabado son intercambiables para ofrecer diversidad de texturas y colores en la fachada.</p>
        </div>
    </div>

    <div class="image-container">
        <img src={imgprueba} alt="">
    </div>
</div>

<style>
   /* .container {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
    }

    .cards-container {
        width: 70%;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .card {
        width: 45%;
        background-color: #f5f5f5;
        border-radius: 10px;
        padding: 20px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        margin-bottom: 20px;
    }

    .image-container {
        width: 30%;
        margin-left: 20px;
    }

    img {
        width: 100%;
        height: auto;
        border-radius: 10px;
    }*/
   .container {
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

   .image-container {
       width: 50%;
       margin-left: 40px;
       object-fit: cover;
   }

   img {
       width: 100%;
       height: auto;
       border-radius: 10px;
   }
</style>
