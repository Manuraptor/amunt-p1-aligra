
<script>
    import imgPortada from "$lib/imagenes/AligraQueEs/Repte urbà_Aligra_2.jpg"
    import { fly } from 'svelte/transition'
    import { afterUpdate } from 'svelte';

    let showDiv = false;

    afterUpdate(() => {
        showDiv = true;
    });
</script>



<main>

    <img src={imgPortada} alt="que-es-Aligra" />

{#if showDiv}
    <div transition:fly={{ x: -400, duration: 1500 }}>

        <h1>ALIGRA</h1>
        <h3>Regeneració Sostenible d'Edificis d'Habitatges</h3>
    </div>
{/if}

</main>


<style>

    main {
        margin: 0;
        height: auto;
        overflow: hidden;
    }
    h1{
        font-family: Impact,sans-serif;
        color: #FCB900;
        font-size: 44px;
        font-weight: lighter;
        letter-spacing: 0.1rem;
    }
    h3{
        color: white;
        font-size: 24px;
        margin-top: -20px;
        letter-spacing: 0.1rem;
    }


    img {
        width: 100vw;
        height: 100vh;
        object-fit: cover;
        object-position: center;
        position: absolute;
        top: 0;
        left: 0;
        z-index: -1;
    }

    div {
        display: flex;
        flex-direction: column;
        position: absolute;
        padding: 15px;
        margin-top: -190px;
        text-align: center;
        transform: translateX(7%);

    }



    @media screen and (min-width: 1920px) {
        div {
            transform: translateX(47%);
            margin-top: -130px;

        }
    }


    /*Version Tablet*/
    @media screen and (min-width: 769px) and (max-width: 1024px) {
        div {
            transform: translateX(10%);
            margin-top: -100px;
        }

    }
    /*Version movil*/
    @media screen and (max-width: 768px) {
        div {
            transform: translateX(0);
           margin-top: -70px;

        }


    }


</style>


