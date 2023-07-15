
<script>
    import { fade } from 'svelte/transition';
    import imgPortada1 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra1.jpg";
    import imgPortada2 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra2.jpg";
    import imgPortada3 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra3.jpg";
    import imgPortada4 from "$lib/imagenes/AligraQueEs/ImgPortadaAligra4.jpg";
</script>

<main>

    <div>
        <article>
            <span class="aligra">Aligra</span> és un dels projectes guanyadors de la convocatòria per a la “Regeneració d’edificis d’habitatges amb sistemes innovadors sostenibles” de la fundació BitHàbitat. En el marc dels “reptes urbans”, l'Ajuntament de Barcelona busca solucions integrals que millorin l'habitabilitat i el rendiment energètic dels habitatges de la ciutat.<br>
            L'objectiu d'aquest “repte urbà” ha estat trobar noves solucions integrals per a millorar el rendiment energètic dels habitatges de Barcelona, aportant nous materials i/o usos dels existents, noves tecnologies i nous dissenys. Amb aquest repte, promogut per BIT Hàbitat, de la mà de l’Institut Municipal d’Urbanisme i la Gerència d’Urbanisme, es buscaven solucions que no només abordin la rehabilitació integral dels edificis sinó que també qüestions com l’ús eficient dels recursos, la mitigació i adaptació al canvi climàtic, així com la resiliència.
        </article>

        <section>
            <img transition:fade src={imgPortada1} alt="">
            <img transition:fade src={imgPortada2} alt="">
            <img transition:fade src={imgPortada3} alt="">
            <img transition:fade src={imgPortada4} alt="">
        </section>

        <article>
            El sistema Aligra respon al Repte Urbà de forma rigorosa i flexible. Diverses empreses de
            perfils complementaris ens hem aliat per oferir aquesta solució multicapa i escalable a partir
            de la nostra llarga experiència acumulada en el disseny arquitectònic amb perspectiva
            ecològica.<br> El resultat és un sistema integrat de construcció prefabricada a base d’elements
            bidimiensonals (2D), que aprèn de les solucions propietàries més interessants que ja ofereix
            el mercat, però que es tradueix a un sistema genèric, de codi obert, adaptable a qualsevol
            licitació o situació constructiva sense les restriccions imposades per les patents privatives.<br>
            </article>
        <article>
            <span class="aligra">Aligra</span> està concebut per adaptar-se a una gran diversitat de situacions, tant a escala arquitectònica com a nivell de paisatge urbà. S’han analitzat diferents configuracions d’ampliació de volum a partir d’edificis reals de la ciutat de Barcelona, des de polígons residencials fins a finques de l'Eixample, passant per alguns casos menys habituals d’edificis no alineats a carrer.<br>
            S’han considerat i analitzat casos d’ampliació de l'espai privatiu dels habitatges, d'introducció de galeries, de generació d’espais oberts privats i col·lectius, així com la possibilitat d’encabir nous nuclis de comunicació vertical. A nivell de materials, es proposa un sistema on les capes d'acabat són intercanviables per tal d'oferir diversitat de textures i colors de façana.
        </article>
    </div>
</main>

<style>
    main {
        margin-left: 210px;
        padding: 25px;
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
        filter: grayscale(90%);
        transition: all 0.5s ease;
    }
    section img:hover{
        filter: none;
    }
    span.aligra{
        font-family: Impact;
       /* color: #FFF455;*/
        color: white;
        letter-spacing: 2px;
        font-size: 20px;
        font-weight: lighter;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;

    }
</style>

