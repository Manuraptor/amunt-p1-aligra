<script>
    import Footer from "/src/lib/componentes/Footer.svelte";
    import '/src/global.css'
    import Caracteristiques from "/src/lib/componentes/Caracteristiques.svelte";

    import Navbar from "$lib/componentes/Navbar.svelte";

</script>
<Navbar />

<Caracteristiques />
<slot />
<Footer />