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
                <div>Aqui van 1 cuadrado y 1 parrafo</div>
            </div>
            <div class="contenedormediano3">
                <img class="square" src={Rectangle27}
                     alt="decoración cuadrado"/>
                <div>Aqui van 1 cuadrado y 1 parrafo</div>
            </div>
        </div>
        <img src={Foto2} alt="foto"/>
    </div>

    <div class="contenedormediano">
        <img src={Foto1}
             alt="foto"/>
        <div class="contenedormediano2">
            <div class="contenedormediano3">

                <div>Aqui van 1 cuadrado y 1 parrafo</div>
                <img class="square" src={Rectangle18}
                     alt="decoración cuadrado"/>
            </div>
            <div class="contenedormediano3">
                <div>Aqui van 1 cuadrado y 1 parrafo</div>
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
                <div>Aqui van 1 cuadrado y 1 parrafo</div>


            </div>
            <div class="contenedormediano3">
                <img class="square" src={Rectangle15}
                     alt="decoración cuadrado"/>
                <div>Aqui van 1 cuadrado y 1 parrafo</div>
            </div>
        </div>
        <img src={Foto3}
             alt="foto"/>
    </div>

</section>

<style>

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
    }

</style>


