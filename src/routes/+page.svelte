

<script>
    import imgPortada from "$lib/imagenes/Portada/Repte urbà_Aligra_2.jpg"
    import { fly } from 'svelte/transition'
    import { afterUpdate } from 'svelte';

    let showDiv = false;

    afterUpdate(() => {
        showDiv = true;
    });
</script>

<img src={imgPortada} alt="que-es-Aligra"  />

{#if showDiv}
    <div transition:fly={{ x: -100, duration: 1000 }}>
        <h2>Regeneració Sostenible d'Edificis d'Habitatges</h2>
        <h4><span>Aligra</span>, la solució guanyadora del repte urbà proposa una renovació avantguardista i sostenible d'edificis residencials mitjançant sistemes innovadors.</h4>
    </div>
{/if}

<style>
    img {
        margin-top: -400px;
        width: 100%;
        height: 800px;
        object-fit: fill;
    }

    div {
       margin-top: -170px;
        height: 110px;
        width: 1000px;
        padding: 20px;
        border-radius: 10px;
        text-align: center;
        transform: translatex(30%);
        transition: transform 0.1s ease;
       /*background-color: rgba(0, 0, 0, 0.2);*/
        background-color: rgba(141, 170, 204, 0.7);
        color: white;

    }

    h2 {
        font-size: 30px;
        margin-bottom: 10px;
    }

    h4 {
        font-size: 18px;
    }
    span{
        font-family: Impact;
        font-weight: lighter;
        letter-spacing: 1px;
        font-size: 20px;
    }
</style>


