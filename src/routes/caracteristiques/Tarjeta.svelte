
<script>
    import Rectangle29 from "$lib/imagenes/Caracteristiques/Rectangle29.jpg"
    import Rectangle27 from "$lib/imagenes/Caracteristiques/Rectangle27.jpg"
    import Foto2 from "$lib/imagenes/Caracteristiques/d21.jpg"

</script>




<Tarjeta>
    <div class="contenedorgrupo">
        <div class="contenedor2cuadrados">
            <div class="cuadradoytexto">
                <img class="square" src={Rectangle29}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">
                    -Economia de mitjans.

                    El sistema multicapa, concebut de manera que cada estrat
                    compleix alhora diverses funcions, ofereix el màxim rendiment
                    dels materials.
                </div>
            </div>
            <div class="cuadradoytexto">
                <img class="square" src={Rectangle27}
                     alt="decoración cuadrado"/>
                <div class="contenedortexto">-
                    Modularitat.

                    Dimensionalment, tant la part física de Aligra com els seus sistemes
                    de serveis es basen rigorosament en modulatges compatibles amb els
                    estàndars industrials i tecnològics més universals.
                </div>
            </div>
        </div>
        <img src={Foto2} alt="foto"/>
    </div>
</Tarjeta>

<style>

    .contenedortexto {

        height: 100px;
        width: 565px;
        display: flex;
        align-items: center;

    }

    .contenedorgrupo {
        display: flex;
        flex-direction: row;
        margin-top: 80px;
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
        width: 725px;
    }
    </style>