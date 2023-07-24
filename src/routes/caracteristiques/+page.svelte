<script>
    import { fade } from 'svelte/transition';
    import Foto1 from "$lib/imagenes/Caracteristiques/d18.jpg"
    import Foto2 from "$lib/imagenes/Caracteristiques/d21.jpg"
    import Foto3 from "$lib/imagenes/Caracteristiques/foto3carateristiques.jpg"
    import ArticleQueEsAligra from "$lib/componentes/ArticleQueEsAligra.svelte";

</script>




        <h2>Característiques Innovadores del Sistema Arquitectònic &nbsp<span>Aligra</span></h2>



<section>
    <div class="texto">
    <ArticleQueEsAligra>

                   <h2>Economia de mitjans</h2>

                   <p> El sistema multicapa, concebut de manera que cada estrat compleix alhora diverses funcions, ofereix el màxim rendiment dels materials. Amb aquesta filosofia s'han dissenyat elements constructius polivalents que poden combinar-se de manera diversa per assolir finalitats diferents.</p>
    </ArticleQueEsAligra>

      <ArticleQueEsAligra>
                  <h2> Modularitat.</h2>

               <p> Dimensionalment, la part física del sistema està basat en un mòdul de 60 cm, una mida molt compatible amb els actuals estàndards industrials i de transport. El mateix criteri de composició modular s’ha seguit pel que fa a instalꞏlacions, inclosa la sensorització i el software que es proposa.</p>
       </ArticleQueEsAligra>
    </div>
        <img class="fotocaracteristicas" transition:fade src={Foto2} alt="foto"/>

</section>
<section>

        <img class="fotocaracteristicas" transition:fade src={Foto1} alt="foto"/>
    <div class="texto">
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
    <div class="texto">

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
        <img class="fotocaracteristicas" transition:fade src={Foto3} alt="foto"/>


</section>



<style>

   h2{
       display: flex;
       align-items: center;
       justify-content: center;
       margin-bottom: 40px;
   }
   span{
       color: #FCB900;
   }

   .texto{
       display: flex;
       flex-direction: column
   }

    section {
        width: 100%;
        height: 400px;
        display: flex;
        justify-content: space-around;
        margin-top: 120px;
        gap: 30px;
align-items: center;

    }


   img {
       width: 300px;
       height: 380px;
        filter: grayscale(75%);
        transition: all 0.5s ease;
        object-fit: cover;
        cursor:pointer;
row-gap: 200px;

    }
    img:hover {
        filter: none;
        transform: scale(1.1);
    }

</style>


