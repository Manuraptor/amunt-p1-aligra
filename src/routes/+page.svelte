
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
<img src={imgPortada} alt="que-es-Aligra"  />


{#if showDiv}
    <div transition:fly={{ x: -400, duration: 1500 }}>

        <h2>Regeneració Sostenible d'Edificis d'Habitatges</h2>
        <h4><span class="aligra">Aligra</span>, la solució guanyadora del repte urbà proposa una renovació avantguardista i sostenible d'edificis<br> residencials mitjançant sistemes innovadors.</h4>
    </div>
{/if}
</main>

<style>
   img {
       width: 1550px;
       height: 720px;
       object-fit: fill;
       margin-left: -190px;
       margin-top: -190px;
   }


    div {
        display: flex;
        flex-direction: column;
       position: absolute;
      margin-top: -710px;
       margin-left: -120px;
        width: 65%;
       padding: 20px;
        text-align: center;
        transform: translateX(23%);
        transition: transform 0.1s ease;
    }


    h2 {
        color: white;
    }
    h4 {
        color: white;
        margin-top:-5px;
        font-size: 17px;
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
</style>
