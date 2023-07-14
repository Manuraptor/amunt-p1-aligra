
<script>
    import imgLogo from "$lib/imagenes/Logo/AligraLogo.png"
    import '/src/global.css'
    import imgFavicon from "$lib/imagenes/Logo/favicon-navbar.png"




</script>
<nav>
   <!-- <div>
        <img src={imgFavicon} alt="Favicon" class="favicon">
    </div>-->
    <ul>
        <li>
            <a href="/" aria-label="Inicio">
                <img src={imgLogo} alt="LogotipoAligra" class="logo">
            </a>
        </li>

        <li>
            <a href="/Aligra">Què és?</a>
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


    </ul>
    <div>
        <img src={imgFavicon} alt="Favicon" class="favicon">
    </div>
</nav>


<style>
   nav {
        position: absolute;
        align-items: center;
        width: 225px;
        height: 100%;
        background: #131111;
        left: -13%;
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
        color: #FFF455;
        text-decoration: none;
        font-style: normal;
        font-size: 22px;

    }
    nav ul li a:hover{
        font-weight: bold;
        /* background: #DAA600;*/
        background: #FFD700;
        color: white;
        padding: 10px 20px;

    }

    .logo {
        height: 50px;
        width: 50px;
        border-radius: 50%;
    }
   div{
       margin-left: 220px;
       background: #FFF455;
   }
   .favicon {
       height: 50px;
       width: 50px;
   }



</style>