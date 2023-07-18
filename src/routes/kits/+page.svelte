<script>
    import KitCard from '$lib/componentes/KitCard.svelte';
    import Imagen1 from "$lib/imagenes/kits/ImgKit1.jpg";
    import Imagen2 from "$lib/imagenes/kits/ImgKit2.jpg";
    import Imagen3 from "$lib/imagenes/kits/ImgKit3.jpg";
    import Imagen4 from "$lib/imagenes/kits/ImgKit4.jpg";
    import Imagen5 from "$lib/imagenes/kits/ImgKit5.jpg"


    let kits = [
        {
            image: Imagen1,
            title: 'D’AMPLIACIÓ DE VOLUM',
            description: [
                "Modularitat adaptable.",
                "Es tracta d'un sistema modular bidimensional, lleuger i en sec, desmuntable i reutilitzable, basat principalment en fusta microlaminada.",
                "La modulació proposada permet resoldre fàcilment diverses mides d'ampliació.",
                "Economia material.",
                "El sistema es diferencia d'altres solucions basades en fusta per la reducció",
                "de l’ús de material, en un exercici d'optimització radical dels recursos mitjançant l'aprofitament",
                "de les tècniques més avançades de la indústria de la fusta.",
                "Prestacions estructurals i acústiques.",
                "La combinació d'un entramat lleuger de fusta amb una capa de compressió de formigó armat",
                "colꞏlaborant permet millorar alhora les prestacions estructurals i acústiques del mòdul de forjat."
            ]
        },
        {
            image: Imagen2,
            title: 'D’ENVOLUPANT BIOCLIMÀTICA.',
            description: [
                "Sistema modular amb diferents combinacions possibles, adaptable, segons s'agreguin o substitueixin materials, per a obra nova, rehabilitació, espais habitables i espais bioclimàtics.",
                "Es diferencia de les alternatives existents en el mercat (SATEs de construcció in situ, humida, amb materials d'alt impacte ambiental i no recuperables) per la seva concepció en sec, reversible i amb materials recuperables.",
                "Sistema industrialitzat off-site, fabricat en taller, dissenyat en tecnologia BIM i fabricat mitjançant CAD-CAM i muntat en sec amb unions reversibles."

    ]
        },
        {
            image: Imagen3,
            title: 'ALJUB',
            description: [
                "Sistema bicapa compost, que integra una safata aljub estructural que pot suportar dos tipus de capa d'acabat superior: una vegetal i una altra transitable, sense perjudici de que en el futur es puguin desenvolupar d’altres tipus.",
                "Usos: l'aigua recuperada per l'aljub serveix pel reg per degoteig de la coberta vegetal i de l'envolupant vegetal en façana.",
                "En cas de pluges torrencials, el sistema desguassa cap als baixants pluvials quan arriba a la seva capacitat màxima.",
                "Commutació de fonts: El reg per degoteig funciona tant amb aigua recuperada de pluja com, en casos d'emergència, amb aigua de xarxa. Aquest mode s'activa amb nivells baixos d'aigua emmagatzemada en l'aljub o quan el sensor de qualitat de l'aigua dóna un senyal per a la seva renovació.",
                "El sistema d'emergència s'encarregad'emplenar l'aljub fins a aconseguir el nivell d'aigua necessària per al reg diari.",
                "Excés d’aigua: l'aljub porta un sobreeixidor per a la descàrrega d'aigua cap als baixants pluvials.",
                "Adaptabilitat: és monitoritzable i ajustable en quantitat i freqüència de reg per l'usuaria través de l'app del kit smart building."

    ]
        },
        {
            image: Imagen4,
            title: 'FOTOVOLTAIC',
            description: [
                "Sistema modular que permetrà la creació d'una comunitat energètica que podrà arribar a subministrar energia per a tot l'edifici.",
                "Solució completament integrada que redueix els problemes associats a la instalꞏlació d'aquesta mena de sistemes en edificis d'habitatges (espai, facilitat d'instalꞏlació, constitució de la comunitat…).",
                "Pèrgola fotovoltaica que permetrà habilitar nous espais ombrejats en la coberta, sense perdre superfície disponible."

            ]
        },
        {
            image: Imagen5;
            title: 'SMART BUILDING',
            description: [
                "Monitoratge i control.",
                "El kit Smart building assumeix el monitoratge constant dels indicadors aportats per múltiples sensors sobre els rendiments ambientals, hídrics i energètics de la pell bioclimàtica, de les plaques fotovoltaiques i de l'aljub.",
                "Quan és necessari, també executa comandaments automàtics de control de les instalꞏlacions per tal de millorar aquests rendiments.",
                "El kit inclou tota la infraestructura necessària per assumir aquestes funcions.",
                "Codi obert.",
                "El sistema de monitorització i control utilitza components de maquinari i programari de codi obert.",
                "Aquests components són econòmics, fàcilment replicables i fins i tot de producció pròpia.",
                "Les funcions de control estan obertes a la gamificació, de manera que la comunitat d'usuaris pugui adoptar pautes responsables de consum d'aigua i energia.",
                "Replicabilitat i escalabilitat.",
                "El kit Smart building es pot integrar com a node descentralitzat dins d'una xarxa de sensors urbans de major escala.",
                "L'ús d'APIs amb diversos graus d'obertura permet intercanviar dades amb l'exterior, preservant sempre la privadesa dels usuaris.",
                "Això permet escalar el programari utilitzat, que pot connectar en xarxa múltiples nodes capaços d'interactuar entre si, tot federant o centralitzant les dades intercanviades.",
                "L'aplicació Docker garantirà que el sistema es pugui replicar i escalar."

            ]
        }
    ];
</script>
<main>
    <div>
        {#each kits as kit,i}
            <KitCard numero={i} {kit} />
        {/each}
    </div>
</main>

<style>

    div{
        display: grid;
        grid-template-columns: (5, 1fr);
        gap: 20px;
        padding: 60px;
        padding-top: 70px;

    }



</style>

