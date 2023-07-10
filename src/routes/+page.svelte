<script>
    import imgPortada from "$lib/imagenes/Portada/Repte urbà_Aligra_2.jpg"
    import imgPortada1 from "$lib/imagenes/Portada/ImgPortadaAligra1.jpg"
    import imgPortada2 from "$lib/imagenes/Portada/ImgPortadaAligra2.jpg"
    import imgPortada3 from "$lib/imagenes/Portada/ImgPortadaAligra3.jpg"
    import imgPortada4 from "$lib/imagenes/Portada/ImgPortadaAligra4.jpg"
</script>

    <img src={imgPortada} alt="portada">
    <h2>Projecte Aligra</h2>
    <h3>UNA SOLUCIÓ ALTERNATIVA D'ACCÉS A L'HABITATGE PÚBLIC</h3>

<article>
    <span class="aligra">Aligra</span> és un dels projectes guanyadors de la convocatòria per a la “Regeneració d’edificis d’habitatges amb sistemes innovadors sostenibles” de la fundació BitHábitat. En el marc dels “reptes urbans”, l'Ajuntament de Barcelona busca solucions integrals que millorin l'habitabilitat i el rendiment energètic dels habitatges de la ciutat.<br> <span class="objectiu">L'objectiu </span>d'aquest “repte urbà” ha estat trobar noves solucions integrals per a millorar el rendiment energètic dels habitatges de Barcelona, aportant nous materials i/o usos dels existents, noves tecnologies i nous dissenys. Amb aquest repte, promogut per BIT Hàbitat, de la mà de l’Institut Municipal d’Urbanisme i la Gerència d’Urbanisme, es buscaven solucions que no només abordin la rehabilitació integral dels edificis sinó que també qüestions com l’ús eficient dels recursos, la mitigació i adaptació al canvi climàtic, així com la resiliència.

</article>
<section>
<img src={imgPortada1} alt="">
<img src={imgPortada2} alt="">
<img src={imgPortada3} alt="">
<img src={imgPortada4} alt="">
</section>

<article>
    <span class="sistema">El sistema</span> Aligra respon al Repte Urbà de forma rigorosa i flexible. Diverses empreses de
    perfils complementaris ens hem aliat per oferir aquesta solució multicapa i escalable a partir
    de la nostra llarga experiència acumulada en el disseny arquitectònic amb perspectiva
    ecològica. <br><span class="resultat">El resultat</span> és un sistema integrat de construcció prefabricada a base d’elements
    bidimiensonals (2D), que aprèn de les solucions propietàries més interessants que ja ofereix
    el mercat, però que es tradueix a un sistema genèric, de codi obert, adaptable a qualsevol
    licitació o situació constructiva sense les restriccions imposades per les patents privatives.<br>
    <span class="aligra">Aligra</span> està concebut per adaptar-se a una gran diversitat de situacions, tant a escala
    arquitectònica com a nivell de paisatge urbà. S’han analitzat diferents configuracions
    d’ampliació de volum a partir d’edificis reals de la ciutat de Barcelona, des de polígons
    residencials fins a finques de l'Eixample, passant per alguns casos menys habituals d’edificis
    no alineats a carrer.<br> S’han considerat i analitzat casos d’ampliació de l'espai privatiu dels
    habitatges, d'introducció de galeries, de generació d’espais oberts privats i colꞏlectius, així
    com la possibilitat d’encabir nous nuclis de comunicació vertical. A nivell de materials, es
    proposa un sistema on les capes d'acabat són intercanviables per tal d'oferir diversitat de
    textures i colors de façana.

</article>


<style>
    img{
        width:100%;
        height:600px;
        border-bottom: 20px solid rgba(252, 185, 0, 1);
    }
    h2{
        width: 486px;
        color: rgba(252,185,0,1);
        position: absolute;
        top: 35px;
        left: 200px;
        font-weight: Bold;
        font-size: 35px;
        opacity: 1;
        text-align: center;
        text-decoration: none;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
    }
    h3{
        width: 780px;
        color: rgba(252,185,0,1);
        position: absolute;
        top: 520px;
        left: 420px;
        font-weight:bold;
        font-style: italic;
        font-size: 25px;
        opacity: 1;
        text-align: center;
        text-decoration: none;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
    }
    article{
        color: black;
        font-weight:normal;
        font-size: 20px;
        opacity: 1;
        text-align: justify;
        margin: 20px 15px 20px 215px;
    }
    article span.aligra {
        display: inline-block;
        margin-left: 30px;
        text-align: center;
        font-weight: bold;
        font-size: 25px;
        color: rgba(252, 185, 0, 1);
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
    }
    article span.objectiu{
        margin-left: 30px;
    }
    section{
        display: flex;
        overflow-x: auto;
        margin-left: 215px;
       /* scroll-snap-type: x mandatory;*/
        gap: 10px;
        margin-bottom: 10px;
        padding-right: 10px;
      /*  scroll-behavior: smooth;*/
    }

    section img{
        width: 300px;
        height: 200px;
        scroll-snap-align: center;
        transition: transform 0.3s ease;
    }
    article span.resultat{
        margin-left: 30px;
    }
    article span.sistema{
        margin-left: 30px;
    }



</style>
