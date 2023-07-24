
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
            <h2>Regeneració Sostenible d'Edificis d'Habitatges</h2>
            <h4><span class="aligra">Aligra</span>, la solució guanyadora del repte urbà proposa una renovació avantguardista i sostenible d'edificis<br> residencials mitjançant sistemes innovadors.</h4>
        </div>
    {/if}
</main>


<style>

    main {
        margin: 0;
        height: auto;
        overflow: hidden;
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
        margin-top: -170px;
        text-align: center;
        transform: translateX(27%);

    }

    h2 {
        color: white;
    }
    h4 {
        color: white;
       margin-top:-5px;
        font-size: 16px;
    }

    @media screen and (min-width: 1920px) {
        div{
            transform: translateX(37%);
            margin-top: -130px;

        }
        h4{
            font-size: 20px;
        }
    }
    /*Version Tablet*/
    @media screen and (min-width: 769px) and (max-width: 1024px) {
        div {
            transform: translateX(10%);
            margin-top: -100px;
        }
        h2{
            font-size: 19px;
        }
        h4 {
            font-size: 14px;
        }
        .aligra{
            font-size: 15px;
        }
    }
    /*Version movil*/
    @media screen and (max-width: 768px) {
        div {
            transform: translateX(0);
           margin-top: -70px;
        }
        h2{
            font-size: 19px;
        }

        h4 {
            font-size: 14px;
        }
        .aligra{
            font-size: 14px;
        }
    }


</style>


