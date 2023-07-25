<script>
    import KitCard from "$lib/componentes/KitCard.svelte";
    import Imagen1 from "$lib/imagenes/kits/ImgKit6.jpg";
    import Imagen2 from "$lib/imagenes/kits/ImgKit7.jpg";
    import Imagen3 from "$lib/imagenes/kits/ImgKit8.jpg";
    import Imagen4 from "$lib/imagenes/kits/ImgKit9.jpg";
    import Imagen5 from "$lib/imagenes/kits/ImgKit10.jpg"



    const kits = [
        {
            title: 'KIT 1',
            image: Imagen1,
            link: '/kitPage1',
        },
        {
            title: 'KIT 2 ',
            image: Imagen2 ,
            link: '/kitPage2',
        },
        {
            title: 'KIT 3 ',
            image: Imagen3,
            link: '/kitPage3',
        },
        {
            title: 'KIT 4',
            image: Imagen4 ,
            link: '/kitPage4',
        },
        {
            title: 'KIT 5',
            image: Imagen5 ,
            link: '/kitPage5',
        },
    ];

</script>

<main>
     {#each kits as kit}

         <KitCard title={kit.title} image="{kit.image}" link={kit.link} />
     {/each}

</main>

<style>

    main {
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        grid-template-rows: repeat(5, 120%);
        gap: 5px;

    }

</style>
