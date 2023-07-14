<script>
    import '/src/global.css'

    import Componente from "$lib/componentes/Componente.svelte";


</script>

<main>

    <Componente/>


</main>


<style>

    main {
        width: 100%;
        padding-top: 180px;
    }

 .textoylogo{

      display: flex;
     flex-direction: row;
     justify-content: space-around;
     height: 100px;
     width: 900px;
     gap:85px;
     margin-left: 275px;
 }

 .contenedortexto{


     display: flex;
     align-items: center;
     height: 100px;
     width: 730px;

 }

</style>