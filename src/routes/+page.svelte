<script>
    import imgPortada from "$lib/imagenes/Portada/Repte urbà_Aligra_2.jpg"

    let sidebarActive;

</script>
    <main>
    <img src={imgPortada} alt="portada">
        <header class:shifted={sidebarActive}>
    <h2 class="portada-heading">Projecte Aligra</h2>
    <h3 class="portada-heading">UNA SOLUCIÓ ALTERNATIVA D'ACCÉS A L'HABITATGE PÚBLIC</h3>
        </header>
</main>

<style>
    main{
        overflow: hidden;
    }
    img{
        width:100%;
        height:641px;
        border-bottom: 20px solid rgba(252, 185, 0, 1);
    }

    header {
        position: relative;
        transition: left 0.3s ease;
        left: 0;
    }

    header.shifted {
        left: 170px;
    }

    h2.portada-heading {
        width: 486px;
        color: rgba(252, 185, 0, 1);
        position: absolute;
        /*top: -620px;*/
        bottom: 580px;
        left: 170px;
        font-family: Impact;
        font-weight: lighter;
        font-size: 30px;
        letter-spacing: 2px;
        text-align: center;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
        transition: left 0.8s ease;
    }

    header.shifted h2.portada-heading {
        left: 0;
    }

    h3.portada-heading {
        width: 780px;
        color: rgba(252, 185, 0, 1);
        position: absolute;
        top: -65px;
        left: 280px;
        font-weight: bold;
        font-style: italic;
        font-size: 25px;
        opacity: 1;
        text-align: center;
        text-decoration: none;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
        transition: left 0.8s ease;
    }

    header.shifted h3.portada-heading {
        left: -10px;
    }




</style>
