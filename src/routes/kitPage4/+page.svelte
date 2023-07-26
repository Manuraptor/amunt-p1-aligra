<script>
    import {fade} from 'svelte/transition';
    import Imagen4 from "$lib/imagenes/kits/ImgKit4.jpg";
</script>

<section>
    <div>
        <h2>Kit 4: Fotovoltaic</h2>
        <p>Sistema modular que permetrà la creació d'una comunitat energètica que podrà arribar a subministrar energia
            per a tot l'edifici.
            Solució completament integrada que redueix els problemes associats a la instalꞏlació d'aquesta mena de
            sistemes en edificis d'habitatges (espai, facilitat d'instalꞏlació, constitució de la comunitat…).
            Pèrgola fotovoltaica que permetrà habilitar nous espais ombrejats en la coberta, sense perdre superfície
            disponible.
        </p>
    </div>
    <img class="ImgKit4" transition:fade src={Imagen4} alt="foto"/>
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