

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

        width: 100%;
        height: 740px;
        /*object-fit: fill;*/
        object-fit: cover;
    }

    div {
        display: flex;
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
        font-size: 18px;
        margin-left: 110px;
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


