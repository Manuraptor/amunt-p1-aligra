<script>
    import {fade} from 'svelte/transition';
    import Imagen2 from "$lib/imagenes/kits/imgKit2.jpg"
</script>

<section>
    <div>
        <h2>Kit 2: d’envolupant bioclimàtica</h2>
        <p>Sistema modular amb diferents combinacions possibles, adaptable, segons s'agreguin o substitueixin materials,
            per a obra nova, rehabilitació, espais habitables i espais bioclimàtics.
            Es diferencia de les alternatives existents en el mercat (SATEs de construcció in situ, humida, amb materials
            d'alt impacte ambiental i no recuperables) per la seva concepció en sec, reversible i amb materials recuperables.
            Sistema industrialitzat off-site, fabricat en taller, dissenyat en tecnologia BIM i fabricat mitjançant
            CAD-CAM i muntat en sec amb unions reversibles.
        </p>
    </div>

    <img class="ImgKit2" transition:fade src={Imagen2} alt="foto"/>
</section>

<style>

    div{
        background-color: #f5f5f5;
        border-radius: 10px;
        padding: 20px;
        text-align: justify;
        margin-bottom: 50px;
    }

    img{
        width: 800px;
        height: 650px;
        object-fit: contain;
        margin-top: -20px;
        transition: all 0.5s ease;
    }

    img:hover {
        transform: scale(1.1);
        filter: none;
    }

</style>
