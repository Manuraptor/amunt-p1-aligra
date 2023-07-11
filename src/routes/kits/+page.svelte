<script>
     import  ImgKit1  from "$lib/imagenes/kits/ImgKit1.jpg";
     import  ImgKit2  from "$lib/imagenes/kits/ImgKit2.jpg";
     import  ImgKit3  from "$lib/imagenes/kits/ImgKit3.jpg";
     import  ImgKit4  from "$lib/imagenes/kits/ImgKit4.jpg";
     import  ImgKit5  from "$lib/imagenes/kits/ImgKit5.jpg";
     import '/src/global.css'
</script>

<section>

    <h1>Parts que componen el sistema Aligra</h1>
    <div class="articulos">

        <img src={ImgKit1} alt="kits">
        <p>· Kit 1: d’ampliació de volum<br>
              · Modularitat adaptable. Es tracta d'un sistema modular bidimensional, lleuger i en sec,<br>
                desmuntable i reutilitzable, basat principalment en fusta microlaminada. La modulació <br>
                proposada permet resoldre fàcilment diverses mides d'ampliació.<br>
              · Economia material. El sistema es diferencia d'altres solucions basades en fusta per la<br>
                reducció de l’ús de material, en un exercici d'optimització radical dels recursos mitjançant<br>
                l'aprofitament de les tècniques més avançades de la indústria de la fusta.<br>
        </p>


        <p>Kit 2: d’envolupant bioclimàtica
            Sistema modular amb diferents combinacions possibles, adaptable, segons s'agreguin o substitueixin materials, per a obra nova, rehabilitació, espais habitables i espais bioclimàtics.
            Es diferencia de les alternatives existents en el mercat (SATEs de construcció in situ, humida, amb materials d'alt impacte ambiental i no recuperables) per la seva concepció en sec, reversible i amb materials recuperables.
            Sistema industrialitzat off-site, fabricat en taller, dissenyat en tecnologia BIM i fabricat mitjançant CAD-CAM i muntat en sec amb unions reversibles.
        </p>
        <img src={ImgKit2} alt="kits">


        <img src={ImgKit3} alt="kits">
        <p>Kit aljub
            Sistema bicapa compost, que integra una safata aljub estructural que pot suportar dos tipus de capa d'acabat superior: una vegetal i una altra transitable, sense perjudici de que en el futur es puguin desenvolupar d’altres tipus.
            Usos: l'aigua recuperada per l'aljub serveix pel reg per degoteig de la coberta vegetal i de l'envolupant vegetal en façana. En cas de pluges torrencials, el sistema desguassa cap als baixants pluvials quan arriba a la seva capacitat màxima.
            Commutació de fonts: el reg per degoteig funciona tant amb aigua recuperada de pluja com, en casos d'emergència, amb aigua de xarxa. Aquest mode s'activa amb nivells baixos d'aigua emmagatzemada en l'aljub o quan el sensor de qualitat de l'aigua dóna un senyal per a la seva renovació. El sistema d'emergència s'encarregad'emplenar l'aljub fins a aconseguir el nivell d'aigua necessària per al reg diari
            Excés d’aigua: l'aljub porta un sobreeixidor per a la descàrrega d'aigua cap als baixants pluvials.
            Adaptabilitat: és monitoritzable i ajustable en quantitat i freqüència de reg per l'usuaria través de l'app del kit smart building.
        </p>

        <p>Kit fotovoltaic
            Sistema modular que permetrà la creació d'una comunitat energètica que podrà arribar a subministrar energia per a tot l'edifici.
            Solució completament integrada que redueix els problemes associats a la instalꞏlació d'aquesta mena de sistemes en edificis d'habitatges (espai, facilitat d'instalꞏlació, constitució de la comunitat…).
            Pèrgola fotovoltaica que permetrà habilitar nous espais ombrejats en la coberta, sense perdre superfície disponible.

        </p>
        <img src={ImgKit4} alt="kits">


        <img src={ImgKit5} alt="kits">
        <p>Kit Smart building
            Monitoratge i control. El kit Smart building assumeix el monitoratge constant dels indicadors aportats per múltiples sensors sobre els rendiments ambientals, hídrics i energètics de la pell bioclimàtica, de les plaques fotovoltaiques i de l'aljub. Quan és necessari, també executa comandaments automàtics de control de les instalꞏlacions per tal de millorar aquests rendiments. El kit inclou tota la infraestructura necessària per assumir aquestes funcions.
            Codi obert. El sistema de monitorització i control utilitza components de maquinari i programari de codi obert. Aquests components són econòmics, fàcilment replicables i fins i tot de producció pròpia. Les funcions de control estan obertes a la gamificació, de manera que la comunitat d'usuaris pugui adoptar pautes responsables de consum d'aigua i energia.
            Replicabilitat i escalabilitat. El kit Smart building es pot integrar com a node descentralitzat dins d'una xarxa de sensors urbans de major escala. L'ús d'APIs amb diversos graus d'obertura permet intercanviar dades amb l'exterior, preservant sempre la privadesa dels usuaris. Això permet escalar el programari utilitzat, que pot connectar en xarxa múltiples nodes capaços d'interactuar entre si, tot federant o centralitzant les dades intercanviades. L'aplicació Docker garantirà que el sistema es pugui replicar i escalar.
        </p>
    </div>

</section>

<style>
    h1{
        font-size: 24px;
    }

    .articulos {
        display: grid;
        grid-template-columns: repeat(2, 1fr) ;
        margin: 50px 50px;


    }
    img {
        width: 700px;
        height: 350px;
    }
    p{
        padding: 20px 20px;
        width: 700px;

    }



</style>

