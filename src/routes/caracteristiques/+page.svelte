<script>
    import { fade } from 'svelte/transition';
    import Foto1 from "$lib/imagenes/Caracteristiques/f6.jpg"
    import Foto2 from "$lib/imagenes/Caracteristiques/f2.jpg"
    import Foto3 from "$lib/imagenes/Caracteristiques/foto3carateristiques.jpg"
    import ArticleQueEsAligra from "$lib/componentes/ArticleQueEsAligra.svelte";

</script>






<main>
<section>
    <div >
    <ArticleQueEsAligra>

                   <h2>Economia de mitjans</h2>

                   <p> El sistema multicapa, concebut de manera que cada estrat compleix alhora diverses funcions, ofereix el màxim rendiment dels materials. Amb aquesta filosofia s'han dissenyat elements constructius polivalents que poden combinar-se de manera diversa per assolir finalitats diferents.</p>
    </ArticleQueEsAligra>

      <ArticleQueEsAligra>
                  <h2> Modularitat.</h2>

               <p> Dimensionalment, la part física del sistema està basat en un mòdul de 60 cm, una mida molt compatible amb els actuals estàndards industrials i de transport. El mateix criteri de composició modular s’ha seguit pel que fa a instalꞏlacions, inclosa la sensorització i el software que es proposa.</p>
       </ArticleQueEsAligra>
    </div>
        <img class="fotoeconomia" transition:fade src={Foto2} alt="foto"/>

</section>
<section>

        <img class="fotocaracteristicas" transition:fade src={Foto1} alt="foto"/>
    <div class="texto1">
        <ArticleQueEsAligra>
                    <h2>Lleugeresa</h2>

                 <p> La selecció acurada dels materials i l'aprofitament òptim de les seves prestacions permet que el sistema assoleix graus de lleugeresa considerablement superiors als de les alternatives similars que ofereix el mercat. Això millora els processos de muntatge i desmuntatge en matèria de seguretat, inclusivitat i estalvi energètic.
                 </p>
    </ArticleQueEsAligra>

            <ArticleQueEsAligra>
           <h2>Facilitat de muntatge</h2>

                <p> La combinació de lleugeresa i modularitat, juntament amb l'ús d'unions reversibles i accessibles, facilita notablement el muntatge i el desmuntatge dels elements constructius.
                </p>
    </ArticleQueEsAligra>
    </div>
</section>
<section>
    <div>

<ArticleQueEsAligra>
                   <h2>Materials ecològics.</h2>

                 <p>El sistema prioritza l’ús de materials saludables, renovables, reciclables i reutilitzables, principalment materials negatius en CO2, no emissors de COVs, higroscòpics, i materials que no retinguin ni propaguin radiació electromagnètic.</p>

    </ArticleQueEsAligra>
           <ArticleQueEsAligra>
               <h2>Flexibilitat</h2>

                  <p>En oferir una àmplia gamma de materials i gruixos, el sistema
                    facilita l’adaptació a eventuals modificacions amb la possible
                    participació dels futurs usuaris.</p>
           </ArticleQueEsAligra>
    </div>
        <img transition:fade src={Foto3} alt="foto"/>


</section>

</main>

<style>
    main{
        margin: 7rem;
    }

   h2{
       display: flex;
       align-items: center;
       justify-content: center;
       margin-bottom: 20px;
   }


   div{
       display: flex;
       flex-direction: column;
      margin-left: -100px;
   }

    section {
        width: 100%;
        height: 400px;
        display: flex;
        justify-content: space-between;
        margin-top: 250px;
        gap: 70px;
        align-items: center;

    }


   img {
       width: 300px;
       height: 700px;
        filter: grayscale(100%);
       margin-right: -220px;
        transition: all 0.5s ease;
        object-fit: cover;
        cursor:pointer;
       margin-bottom: 4px;

    }
    img:hover {
        filter: none;
        transform: scale(1.1);
    }

    .fotocaracteristicas{
        margin-left: -100px;
    }
    .texto1{
        margin-left: 220px;
        margin-right: -220px;

    }

    @media screen and (min-width: 1920px) {
        main{
            margin: 11rem;
        }
    }
    @media screen and (min-width: 769px) and (max-width: 1024px){
        main{
            margin-left: -80px;
        }
        section{
            width: 370px;
            height: 600px;
            margin-bottom: 150px;
        }
        div{
            pointer-events: none;
        }
    }
    @media screen and (max-width: 768px) {
        main{
            margin-left: -90px;

        }
        section{
            width: 300px;
            height: 400px;

        }
        img{
            width: 200px;

        }
        .fotocaracteristicas{
            margin-left: -90px;
        }
        .texto1{

            margin-right: -270px;
            margin-top:90px;

        }

    }

</style>


