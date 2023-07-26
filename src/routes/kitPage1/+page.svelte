<script>
    import {fade} from 'svelte/transition';
    import Imagen1 from "$lib/imagenes/kits/ImgKit1.jpg";
</script>

    <section>
        <div>
            <h2>Kit 1: D’ampliació de volum</h2>
            <p> Modularitat adaptable. Es tracta d'un sistema modular bidimensional, lleuger i en sec, desmuntable i reutilitzable,
                basat principalment en fusta microlaminada. La modulació proposada permet resoldre fàcilment diverses mides d'ampliació.

                Economia material. El sistema es diferencia d'altres solucions basades en fusta per la reducció de l’ús de material,
                en un exercici d'optimització radical dels recursos mitjançant l'aprofitament de les tècniques més avançades de la indústria de la fusta.

                Prestacions estructurals i acústiques. La combinació d'un entramat lleuger de fusta amb una capa de compressió de formigó armat
                colꞏlaborant permet millorar alhora les prestacions estructurals i acústiques del mòdul de forjat.

            </p>
        </div>
         <img class="ImgKit1" transition:fade src={Imagen1} alt="foto"/>
    </section>

<style>

    div{
        background-color: #f5f5f5;
        border-radius: 10px;
        padding: 20px;
        text-align: justify;
        margin-bottom: 50px;
    }


</style>