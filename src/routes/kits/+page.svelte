<script>
    import KitCard from "$lib/componentes/KitCard.svelte";
    import Imagen1 from "$lib/imagenes/kits/imgKit6.jpg";
    import Imagen2 from "$lib/imagenes/kits/imgKit7.jpg";
    import Imagen3 from "$lib/imagenes/kits/imgKit8.jpg";
    import Imagen4 from "$lib/imagenes/kits/imgKit9.jpg";
    import Imagen5 from "$lib/imagenes/kits/imgKit10.jpg"



    const kits = [
        {
            title: 'KIT 1',
            subtitle:'Modul d´ampliació de volum',
            image: Imagen1,
            link: '/kitPage1',
        },
        {
            title: 'KIT 2 ',
            subtitle:'Modul d´ampliació de volum',
            image: Imagen2 ,
            link: '/kitPage2',
        },
        {
            title: 'KIT 3 ',
            subtitle:'Modul d´ampliació de volum',
            image: Imagen3,
            link: '/kitPage3',
        },
        {
            title: 'KIT 4',
            subtitle:'Modul d´ampliació de volum',
            image: Imagen4 ,
            link: '/kitPage4',
        },
        {
            title: 'KIT 5',
            subtitle:'Modul d´ampliació de volum',
            image: Imagen5 ,
            link: '/kitPage5',
        },
    ];

</script>

<main>
     {#each kits as kit}

         <KitCard title={kit.title} subtitle={kit.subtitle} image="{kit.image}" link={kit.link} />
     {/each}

</main>

<style>

    main {
        display: grid;
        grid-template-columns: repeat(5, 1fr);
        grid-template-rows: repeat(5, 125%);
        gap: 4px;

    }

</style>
