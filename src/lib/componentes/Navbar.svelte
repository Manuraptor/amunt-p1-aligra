<script>
    import '/src/global.css';
    import imgFavicon from "$lib/imagenes/LogoYFaviconesMenu/logoAligra.png";


</script>

<nav>
    <img src={imgFavicon} alt="Favicon" class="favicon">
    <ul>
        <li>
            <a href="/" class="aligra">Aligra
            </a>
        </li>
        <li>
            <a href="/Aligra">Qui som?</a>
        </li>
        <li>
            <a href="/objectiu">Objectiu</a>
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
</nav>

<style>
    nav {
        display: flex;
        position: fixed;
        top: 0;
        bottom: 0;
        align-items: flex-end;
        width: 230px;
        max-height: 100vh;
        flex-direction: column;
        background: rgba(0, 0, 0, 0.6);
        transition: 0.4s linear;
        left: -15%;
    }

    nav:hover {
        left: 0;
    }

    nav ul {
        padding: 0;
    }

    nav ul li {
        list-style: none;
        padding: 15px 10px;
        border-bottom: 1px solid rgba(100, 100, 100, 0.2);
    }

    nav ul li a {
        display: flex;
        justify-content: flex-end;
        margin-right: 18px;
        color: #FCB900;

        text-decoration: none;
        font-weight: normal;
        font-size: 20px;
    }

    nav ul li a:hover {
        cursor: pointer;
        color: white;

    }



    .favicon {
        background-color: #FCB900;
        object-fit: cover;
        position: relative;
        top: 20px;
        left: 36px;
        height: 35px;
        width: 35px;
        border-radius: 50%;
        border: #FCB900;
    }
    .aligra{
        font-size: 25px;
    }
        @media screen and (min-width: 1920px) {
            nav {
                left: -9%;
            }
        }
    /*Version tablet*/
            @media screen and (min-width: 769px) and (max-width: 1024px){
                nav{
                    left:-14.8%;
                }
            }
    /*Version movil*/
    @media screen and (max-width: 768px){

            nav{
                left:-22%;
            }

    }


    /* Estilos para pantallas más pequeñas */
   /* @media screen and (max-width: 768px) {
        nav {
            width: 20%;
            height: 100vh;
            left: 0;
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
            justify-content: center;
        }
    }*/


</style>


