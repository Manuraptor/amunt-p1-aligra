<script>
    import '/src/global.css'
    import Foto1 from "$lib/imagenes/Caracteristiques/d18.jpg"
    import Foto2 from "$lib/imagenes/Caracteristiques/d21.jpg"
    import Foto3 from "$lib/imagenes/Caracteristiques/foto3carateristiques.jpg"
    import Rectangle29 from "$lib/imagenes/Caracteristiques/Rectangle29.jpg"
    import Rectangle27 from "$lib/imagenes/Caracteristiques/Rectangle27.jpg"
    import Rectangle18 from "$lib/imagenes/Caracteristiques/Rectangle18.jpg"
    import Rectangle19 from "$lib/imagenes/Caracteristiques/Rectangle19.jpg"
    import Rectangle14 from "$lib/imagenes/Caracteristiques/Rectangle14.jpg"
    import Rectangle15 from "$lib/imagenes/Caracteristiques/Rectangle15.jpg"
    /* import Tarjeta from "$routes/caracteristiques/Tarjeta.svelte"*/

</script>

<main>
    <article>

    <p><span>Aligra</span> &nbsp està concebut per adaptar-se a una gran diversitat de situacions,</p>
    <p>tant a escala arquitectònica com a nivell de paisatge urbà.</p>


    <h3>Les principals característiques del sistema <span>Aligra</span> són les següents:</h3>

</article>
<!-- <Tarjeta/> -->
<section>
    <div class="contenedorgrupo">
        <div class="contenedor2cuadrados">
            <div class="cuadradoytexto">
                <img src={Rectangle29}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">
                    - Economia de mitjans.

                    El sistema multicapa, concebut de manera que cada estrat
                    compleix alhora diverses funcions, ofereix el màxim rendiment
                    dels materials.
                </div>
            </div>
            <div class="cuadradoytexto">
                <img  src={Rectangle27}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">-
                    Modularitat.

                    Dimensionalment, tant la part física com els seus sistemes de serveis
                    es basen rigorosament en modulatges compatibles amb els estàndars industrials
                    i tecnològics més universals.
                </div>
            </div>
        </div>
        <img src={Foto2} alt="foto"/>
    </div>
</section>
<section>
    <div class="contenedorgrupo">
        <img src={Foto1}
             alt="foto"/>
        <div class="contenedor2cuadrados">
            <div class="cuadradoytexto">

                <div class="contenedortexto">
                    - Facilitat de muntatge.

                    La combinació de lleugeresa i modularitat, juntament
                    amb l’ús d’unions reversibles i accessibles, facilita
                    notablement el seu muntatge i desmuntatge.
                </div>
                <img src={Rectangle18}
                     alt="decoración cuadrado"/>
            </div>
            <div class="cuadradoytexto">
                <div class="contenedortexto">
                    - Lleugeresa.

                    La selecció acurada dels materials i l’aprofitament
                    òptim de les seves prestacions permet millorar els
                    processos de muntatge i desmuntatge en matèria de
                    seguretat, inclusivitat i estalvi energètic.
                </div>
                <img src={Rectangle19}
                     alt="decoración cuadrado"/>
            </div>
        </div>
    </div>
</section>
<section>
    <div class="contenedorgrupo">
        <div class="contenedor2cuadrados">
            <div class="cuadradoytexto">
                <img src={Rectangle14}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">
                    - Materials ecològics.

                    El sistema utilitzat materials negatius en CO2, no emissors de
                    COVs, higroscòpics,i materials que no retenen ni propaguen
                    radiació electromagnètica.
                </div>


            </div>
            <div class="cuadradoytexto">
                <img src={Rectangle15}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">
                    - Flexibilitat.

                    En oferir una àmplia gamma de materials i gruixos, el sistema
                    facilita l’adaptació a eventuals modificacions amb la possible
                    participació dels futurs usuaris.
                </div>
            </div>
        </div>
        <img src={Foto3}
             alt="foto"/>
    </div>

</section>
</main>
<style>


    main {
        margin: 0;
        padding:0;
        box-sizing: border-box;
    }

    article {
        display: flex;
        width: 100%;
        height: 100px;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        padding-top: 250px;
        padding-bottom: 120px;
    }

    section {
        width: 100%;
        display: flex;
        justify-content: center;
        margin-top: 120px;

    }

    .contenedortexto {

        height: 100px;
        width: 730px;
        display: flex;
        align-items: center;

    }

    .contenedorgrupo {
        display: flex;
        flex-direction: row;
    }

    .contenedor2cuadrados {
        display: flex;
        flex-direction: column;
        gap: 50px;
    }

    .cuadradoytexto {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
        height: 100px;
        width: 900px;
        font-size: 20px;
    }

    p {
        display: flex;
        font-size: 36px;
        justify-content: center;

    }

        h3{
            margin-top: 30px;
            font-style: initial;
            font-size: 24px;
            font-weight: lighter;
        }
    span {
        font-family: Impact;
        letter-spacing: 1px;
        font-weight: lighter;
        color: #FFF455;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
    }

</style>


