
<!--
<script>
    import imgPortada from "$lib/imagenes/AligraQueEs/Repte urbà_Aligra_2.jpg"
    import { fly } from 'svelte/transition'
    import { afterUpdate } from 'svelte';

    let showDiv = false;

    afterUpdate(() => {
        showDiv = true;
    });
</script>

<img src={imgPortada} alt="que-es-Aligra"  />

{#if showDiv}
    <div transition:fly={{ x: -400, duration: 1500 }}>

        <h2>Regeneració Sostenible d'Edificis d'Habitatges</h2>
        <h4><span>Aligra</span>, la solució guanyadora del repte urbà proposa una renovació avantguardista i sostenible d'edificis residencials mitjançant sistemes innovadors.</h4>
    </div>
{/if}

<style>
    img {

        width: 100%;
        height: 740px;
        object-fit: fill;

    }

    div {
        display: flex;
        flex-direction: column;
        position: absolute;
        margin-top: -720px;
        height: 110px;
        width: 70%;
        padding: 20px;
        border-radius: 10px;
        text-align: center;
        transform: translateX(23%);
        transition: transform 0.1s ease;
    }


    h2 {
        font-size: 22px;
        margin-bottom: 10px;
        margin-left: 110px;
        color: white;
    }
    h4 {
        margin-left: 110px;
        font-size: 16px;
        color: white;
    }

    span{
        font-family: Impact;
        font-weight: lighter;
        letter-spacing: 1px;
        font-size: 22px;
       color: #FCB900;
    }
    @media screen and (max-width: 768px){
        h2{
            font-size: 17px;
        }
        h4{
            font-size: 12px;
            text-align: center;
        }
        span{
            font-size: 17px;
        }
    }
</style>-->


<script>
    import '/src/global.css'
</script>
<style>

</style>