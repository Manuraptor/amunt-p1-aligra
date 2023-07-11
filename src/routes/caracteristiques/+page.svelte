<script>
    import '/src/global.css'
    import Foto1 from "$lib/imagenes/Caracteristiques/d18.jpg"
    import Foto2 from "$lib/imagenes/Caracteristiques/d21.jpg"
    import Foto3 from "$lib/imagenes/Caracteristiques/f11.jpg"
    import Rectangle29 from "$lib/imagenes/Caracteristiques/Rectangle29.jpg"
    import Rectangle27 from "$lib/imagenes/Caracteristiques/Rectangle27.jpg"
    import Rectangle18 from "$lib/imagenes/Caracteristiques/Rectangle18.jpg"
    import Rectangle19 from "$lib/imagenes/Caracteristiques/Rectangle19.jpg"
    import Rectangle14 from "$lib/imagenes/Caracteristiques/Rectangle14.jpg"
    import Rectangle15 from "$lib/imagenes/Caracteristiques/Rectangle15.jpg"

</script>


<section>
    <article>
        <p> Aligra està concebut per adaptar-se a una gran diversitat de situacions,
            tant a escala arquitectònica com a nivell de paisatge urbà.</p>
        <h3>Les principals característiques del sistema Aligra són les següents:</h3>
    </article>
    <div class="contenedormediano">
        <div class="contenedormediano2">
            <div class="contenedormediano3">
                <img class="square" src={Rectangle29}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">-Economia de mitjans.

                    El sistema multicapa, concebut de manera que cada estrat
                    compleix alhora diverses funcions, ofereix el màxim rendiment
                    dels materials.</div>
            </div>
            <div class="contenedormediano3">
                <img class="square" src={Rectangle27}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">-Modularitat.

                    Dimensionalment, tant la part física de Aligra com els seus sistemes
                    de serveis es basen rigorosament en modulatges compatibles amb els
                    estàndars industrials i tecnològics més universals.
                </div>
            </div>
        </div>
        <img src={Foto2} alt="foto"/>
    </div>

    <div class="contenedormediano">
        <img src={Foto1}
             alt="foto"/>
        <div class="contenedormediano2">
            <div class="contenedormediano3">

                <div class="contenedortexto">-Facilitat de muntatge.

                    La combinació de lleugeresa i modularitat, juntament
                    amb l’ús d’unions reversibles i accessibles, facilita          notablement el seu muntatge i desmuntatge.
                </div>
                <img class="square" src={Rectangle18}
                     alt="decoración cuadrado"/>
            </div>
            <div class="contenedormediano3">
                <div class="contenedortexto">-Lleugeresa.

                    La selecció acurada dels materials i l’aprofitament òptim de
                    les seves prestacions permet millorar els processos de muntatge i desmuntatge
                    en matèria de seguretat, inclusivitat i estalvi energètic.</div>
                <img class="square" src={Rectangle19}
                     alt="decoración cuadrado"/>
            </div>
        </div>
    </div>
    <div class="contenedormediano">
        <div class="contenedormediano2">
            <div class="contenedormediano3">
                <img class="square" src={Rectangle14}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">-Materials ecològics.

                    El sistema utilitzat materials negatius en CO2, no emissors de COVs,
                    higroscòpics,i materials que no retenen ni propaguen  radiació electromagnètica.
                </div>


            </div>
            <div class="contenedormediano3">
                <img class="square" src={Rectangle15}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">-Flexibilitat.

                    En oferir una àmplia gamma de materials i gruixos, el sistema facilita
                    l’adaptació a eventuals modificacions amb la possible participació
                    dels futurs usuaris.</div>
            </div>
        </div>
        <img src={Foto3}
             alt="foto"/>
    </div>

</section>

<style>

    section {

        width:1200px;
        height: 1400px;
    }

        .contenedortexto{

            height: 100px;
            width: 565px;
            display: flex;
            align-items: center;

        }
    .contenedormediano {
        display: flex;
        flex-direction: row;
    }

    .contenedormediano2 {
        display: flex;
        flex-direction: column;
    }

    .contenedormediano3 {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
        height: 100px;
        width:725px;
    }

</style>


