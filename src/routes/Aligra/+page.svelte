
<script>
    import imgPortada1 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra1.jpg";
    import imgPortada2 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra2.jpg";
    import imgPortada3 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra3.jpg";
    import imgPortada4 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra4.jpg";
</script>

<main>
    <header>
        <h2>Presentació del Projecte</h2>
        <h2><span>Aligra</span></h2>
    </header>
    <div>
        <article>
            <span class="aligra">Aligra</span> és un dels projectes guanyadors de la convocatòria per a la “Regeneració d’edificis d’habitatges amb sistemes innovadors sostenibles” de la fundació BitHàbitat. En el marc dels “reptes urbans”, l'Ajuntament de Barcelona busca solucions integrals que millorin l'habitabilitat i el rendiment energètic dels habitatges de la ciutat.<br>
            L'objectiu d'aquest “repte urbà” ha estat trobar noves solucions integrals per a millorar el rendiment energètic dels habitatges de Barcelona, aportant nous materials i/o usos dels existents, noves tecnologies i nous dissenys. Amb aquest repte, promogut per BIT Hàbitat, de la mà de l’Institut Municipal d’Urbanisme i la Gerència d’Urbanisme, es buscaven solucions que no només abordin la rehabilitació integral dels edificis sinó que també qüestions com l’ús eficient dels recursos, la mitigació i adaptació al canvi climàtic, així com la resiliència.
        </article>

        <section>
            <img src={imgPortada1} alt="">
            <img src={imgPortada2} alt="">
            <img src={imgPortada3} alt="">
            <img src={imgPortada4} alt="">
        </section>

        <article>
            <span class="aligra">Aligra</span> està concebut per adaptar-se a una gran diversitat de situacions, tant a escala arquitectònica com a nivell de paisatge urbà. S’han analitzat diferents configuracions d’ampliació de volum a partir d’edificis reals de la ciutat de Barcelona, des de polígons residencials fins a finques de l'Eixample, passant per alguns casos menys habituals d’edificis no alineats a carrer.<br>
            S’han considerat i analitzat casos d’ampliació de l'espai privatiu dels habitatges, d'introducció de galeries, de generació d’espais oberts privats i col·lectius, així com la possibilitat d’encabir nous nuclis de comunicació vertical. A nivell de materials, es proposa un sistema on les capes d'acabat són intercanviables per tal d'oferir diversitat de textures i colors de façana.
        </article>
    </div>
</main>

<style>
    main {
        margin-left: 200px;
        padding: 20px;
    }
    header {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        text-align: center;
        height: 80px;
        font-size: 25px;
        margin-bottom: 30px;
    }
    h2 span{
        font-family: Impact;
        font-weight: lighter;


    }

    div {
        display: flex;
        flex-direction: column;
        gap: 20px;
    }

    article {
        background-color: #f5f5f5;
        border-radius: 10px;
        padding: 20px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        text-align: justify;
    }



    section {
        display: flex;
        overflow-x: auto;
        gap: 10px;
    }

    section img {
        width: 300px;
        height: 200px;
        object-fit: cover;
    }
    span.aligra{
        font-family: Impact;
        color: rgba(252, 185, 0, 1);
        letter-spacing: 2px;
        font-size: 20px;
        font-weight: lighter;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;

    }
</style>

