
<script>
    import imgPortada from "$lib/imagenes/Portada/Repte urbà_Aligra_2.jpg"

    let sidebarActive;
    let overlayActive = false;

    function toggleOverlay() {
        overlayActive = !overlayActive;
    }
</script>
<main>
    <img src={imgPortada} alt="portada" on:click={toggleOverlay} />
    <header class:shifted={sidebarActive}>
        <h2 class="portada-heading">Projecte Aligra</h2>
        <h3 class="portada-heading">UNA SOLUCIÓ ALTERNATIVA D'ACCÉS A L'HABITATGE PÚBLIC</h3>
        <div class:active={overlayActive} class="overlay">
            <h4>Solució Guanyadora: Regeneració Sostenible d'Edificis d'Habitatges</h4>
            <p>La solució guanyadora del repte urbà proposa una renovació avantguardista i sostenible d'edificis residencials mitjançant sistemes innovadors. El seu enfocament integral busca optimitzar recursos, reduir el consum energètic i millorar la habitabilitat, aconseguint espais eficients i amigables amb el medi ambient.</p>
        </div>
    </header>
</main>

<style>
    main {
        overflow: hidden;
    }

    img {
        width: 100%;
        height: 641px;
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
        bottom: 580px;
        left: 170px;
        font-family: Impact;
        font-style: italic;
        font-weight: lighter;
        font-size: 30px;
        letter-spacing: 2px;
        text-align: center;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
        transition: left 0.6s ease-in-out;
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
        left: 105px;
    }

    .overlay {
        position: absolute;
        display: flex;
        align-items: center;
        flex-direction: column;
        width: 70%;
        bottom:30px;
        left: 50%;
        transform: translate(-50%, -50%);
        background-color: rgba(0, 0, 0, 0.7);
        color: lightgray;
        padding: 20px;
        border-radius: 5px;
        opacity: 0;
        transition: opacity 0.3s ease;
    }

    .overlay.active {
        opacity: 1;
    }

    h4{
        font-size: 25px;
        margin-bottom:18px;
    }
    p {
        margin: 0;
    }
</style>
