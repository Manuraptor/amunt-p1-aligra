<script>
    import {fade} from 'svelte/transition';
    import Imagen5 from "$lib/imagenes/kits/ImgKit5.jpg";
</script>

<section>
    <div>
        <h2>Kit 5: Smart Building</h2>
        <p>Monitoratge i control. El kit Smart building assumeix el monitoratge constant dels indicadors aportats per
            múltiples sensors sobre els rendiments ambientals, hídrics i energètics de la pell bioclimàtica, de les
            plaques fotovoltaiques i de l'aljub. Quan és necessari, també executa comandaments automàtics de control de
            les instalꞏlacions per tal de millorar aquests rendiments. El kit inclou tota la infraestructura necessària
            per assumir aquestes funcions.
            Codi obert. El sistema de monitorització i control utilitza components de maquinari i programari de codi
            obert. Aquests components són econòmics, fàcilment replicables i fins i tot de producció pròpia. Les
            funcions de control estan obertes a la gamificació, de manera que la comunitat d'usuaris pugui adoptar
            pautes responsables de consum d'aigua i energia.
            Replicabilitat i escalabilitat. El kit Smart building es pot integrar com a node descentralitzat dins d'una
            xarxa de sensors urbans de major escala. L'ús d'APIs amb diversos graus d'obertura permet intercanviar dades
            amb l'exterior, preservant sempre la privadesa dels usuaris. Això permet escalar el programari utilitzat,
            que pot connectar en xarxa múltiples nodes capaços d'interactuar entre si, tot federant o centralitzant les
            dades intercanviades. L'aplicació Docker garantirà que el sistema es pugui replicar i escalar.
        </p>
    </div>
    <img class="ImgKit5" transition:fade src={Imagen5} alt="foto"/>
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