<script>
    import {fade} from 'svelte/transition';
    import Imagen3 from "$lib/imagenes/kits/ImgKit3.jpg";
</script>

<section>
    <div>
        <h2>Kit 3: Aljub</h2>
        <p>Sistema bicapa compost, que integra una safata aljub estructural que pot suportar dos tipus de capa d'acabat
            superior: una vegetal i una altra transitable, sense perjudici de que en el futur es puguin desenvolupar
            d’altres tipus.
            Usos: l'aigua recuperada per l'aljub serveix pel reg per degoteig de la coberta vegetal i de l'envolupant
            vegetal en façana. En cas de pluges torrencials, el sistema desguassa cap als baixants pluvials quan arriba
            a la seva capacitat màxima.
            Commutació de fonts: el reg per degoteig funciona tant amb aigua recuperada de pluja com, en casos
            d'emergència, amb aigua de xarxa. Aquest mode s'activa amb nivells baixos d'aigua emmagatzemada en l'aljub o
            quan el sensor de qualitat de l'aigua dóna un senyal per a la seva renovació. El sistema d'emergència
            s'encarregad'emplenar l'aljub fins a aconseguir el nivell d'aigua necessària per al reg diari
            Excés d’aigua: l'aljub porta un sobreeixidor per a la descàrrega d'aigua cap als baixants pluvials.
            Adaptabilitat: és monitoritzable i ajustable en quantitat i freqüència de reg per l'usuaria través de l'app
            del kit smart building.
        </p>
    </div>
    <img class="ImgKit3" transition:fade src={Imagen3} alt="foto"/>
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