
<script>
    import imgLogo from "$lib/imagenes/Logo/AligraLogo.png"
    import '/src/global.css'
    import {onMount} from "svelte";
    let sidebarActive = false;

    function toggleSidebar() {
        sidebarActive = !sidebarActive;
    }

    onMount(() => {
        const btnToggle = document.querySelector(".toggle-btn");
        const header = document.querySelector("header");
        btnToggle.addEventListener("click", () => {
            toggleSidebar();
            header.classList.toggle("shifted");
        });
    });
</script>

<div id="sidebar" class:active={sidebarActive}>
    <div class="toggle-btn">
        <span>&#9776;</span>
    </div>
    <ul>
        <li><img src={imgLogo} alt="Logotipo"></li>
        <li>
            <a href="/">Aligra</a>
        </li>
        <li>
            <a href="/què-és?">Què és?</a>
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
</div>

<style>
    #sidebar {
        position: fixed;
        width: 205px;
        height: 100%;
        background: #FCB900;
        left: -200px;
        transition: left 0.3s ease;
    }

    #sidebar.active {
        left: 0;
    }

    #sidebar ul li {
        text-align: center;
        padding: 15px 10px;
        border-bottom: 1px solid rgba(100, 100, 100, 0.3);
    }

    #sidebar ul li a {
        color: black;
        text-decoration: none;
        font-style: oblique;
        font-size: 25px;
    }
    #sidebar ul li a:hover{
        font-weight: bold;
    }

    img {
        height: 50px;
        width: 50px;
        border-radius: 50%;
    }

    .toggle-btn {
        background-color: #FCB900;
        position: absolute;
        left: 230px;
        cursor: pointer;
        top: 20px;
        border-radius: 50%;
    }

    span {
        display: block;
        width: 40px;
        text-align: center;
        font-size: 30px;
    }
</style>