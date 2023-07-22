<script>
    import imgLogo from "$lib/imagenes/LogoYFaviconesMenu/image1logoAligra-removebg-preview.png"
    import '/src/global.css'
    import imgFavicon from "$lib/imagenes/LogoYFaviconesMenu/logoAligra.png"
</script>


<nav>

        <img src={imgFavicon} alt="Favicon" class="favicon">

    <ul>
        <li>
            <a href="/" >
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

</nav>


<style>
    nav {
        display: flex;
        position: fixed;
        top: 0;
        bottom: 0;
       align-items: flex-end;
        width: 180px;
        flex-direction: column;
        background: rgba(0, 0, 0, 0.6);
        transition: 0.4s linear;
        left: -10%;

    }

   nav:hover {
        left: 0;
    }

    nav ul li {
        bottom: 90px;
        list-style: none;
       padding: 15px 10px;
      /* border-bottom: 1px solid rgba(100, 100, 100, 0.2);*/
    }


    nav ul li a {
        display: flex;
        justify-content: flex-end;
        margin-right: 18px;
        color: #FCB900;
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;
        text-decoration: none;
        font-style: normal;
        font-size: 20px;
        top:-90px;
    }

    nav ul li a:hover {
        cursor: pointer;
        color:white;
        /*padding: 10px 20px;*/
        text-shadow: -2px -2px 0 #000, 2px -2px 0 #000, -2px 2px 0 #000, 2px 2px 0 #000;

    }

    .logo {
        height: 3rem;
        width: 3rem;
        border-radius: 50%;
    }



    .favicon {
        margin-right:-30px;
        height: 40px;
        width: 40px;
        border-radius: 50%;
        border: #FCB900;
        margin-top: 60px;

    }
    @media screen and (max-width: 768px) {
        nav {
            width: 20%;
            height: 824px;
            left:0;
            justify-content: center;
        }
        .favicon {
            display: none;
        }
        .logo {
            height: 3rem;
            width: 3rem;
        }
        nav ul {
            margin-top: 40px;
            display: flex;
            flex-direction: column;
        }
        nav ul li {
            padding: 10px;
        }
        nav ul li a {
            font-size: 18px;
        }
    }


    @media screen and (max-width: 480px) {
        nav ul li a {
            font-size: 16px;
        }

    }



</style>
