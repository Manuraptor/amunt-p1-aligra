

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

        <h2><span>Aligra</span> REI sistema Aligra respon al Repte Urbá de forma rigorosa y flexible. Diverses empresas de<br> perfils complementaris ens hem aliat per oferir aquesta solució multicap </h2>
    </div>
{/if}

<style>
    img {
       /* margin-top: -400px;*/
        width: 100%;
        height: 800px;
        /*object-fit: fill;*/
        object-fit: cover;
    }

    div {
        display: flex;
        position: absolute;
      margin-top: -760px;
        height: 110px;
        width: 70%;
        padding: 20px;
        border-radius: 10px;
        text-align: center;
        transform: translateX(23%);
        transition: transform 0.1s ease;
     /*background-color: rgba(0, 0, 0, 0.5);*/
       /*background-color: rgba(141, 170, 204, 0.7);*/
        /*text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;*/

       /* color: hsl(60, 80%, 90%);*/




    }

    h2 {
        font-size: 18px;
        margin-left: 110px;
      /*  margin-bottom: 10px;*/
        color: white;

    }

    span{
        font-family: Impact;
        font-weight: lighter;
        letter-spacing: 1px;
        font-size: 25px;
       color: #FCB900;
    }
</style>


