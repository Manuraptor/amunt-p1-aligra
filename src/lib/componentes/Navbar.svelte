<script>
    import imgLogo from "$lib/imagenes/Logo/AligraLogo.png"
    import '/src/global.css'
    import imgFavicon from "$lib/imagenes/Logo/menu (1).png"
</script>
<nav>

    <ul>
        <li>
            <a href="/" aria-label="Inicio">
                <img src={imgLogo} alt="LogotipoAligra" class="logo">
            </a>
        </li>

        <li>
            <a href="/Aligra">Qui som?</a>
        </li>
        <li>
            <a href="/caracteristiques">Caracteristiques</a>
        </li>
        <li>
            <a href="/kits">Kits</a>
        </li>
        <li>
            <a href="/colaboradors">Colaboradors</a>
        </li>
        <li>
            <a href="/prueba">Prueba</a>
        </li>

    </ul>
    <div>
        <img src={imgFavicon} alt="Favicon" class="favicon">
    </div>
</nav>


<style>
    nav {
       /* position: relative;*/
        position: fixed;
        align-items: center;
        width: 240px;
        height: 100%;
        background: rgba(0, 0, 0, 0.6);
        left: -14%;
        transition: 0.4s linear;

    }

    nav:hover {
        left: 0;
    }

    nav ul li {
        list-style: none;
        text-align: center;
        padding: 15px 10px;
       border-bottom: 1px solid rgba(100, 100, 100, 0.2);
    }


    nav ul li a {
        color: #FCB900;
        text-decoration: none;
        font-style: normal;
        font-size: 22px;

    }

    nav ul li a:hover {
        font-weight: bold;
      /* background: #FFD700;*/
  /* background:hsl(60, 80%, 90%);*/
        /*background: rgba(0, 0, 0, 0.2);*/
        /*background-color: rgba(141, 170, 204, 0.7);*/
        /*color: white;*/
       /* color:hsl(60, 80%, 90%);*/
        padding: 10px 20px;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;

    }

    .logo {
        height: 60px;
        width: 60px;
        border-radius: 50%;
    }

    div {
        margin-left: 220px;
        background: black;
    }

    .favicon {
        height: 40px;
        width: 40px;
        border-radius: 50%;
      /* background: rgba(141, 170, 204, 0.7);*/
        background-color: hsl(60, 80%, 90%);

    }


</style>