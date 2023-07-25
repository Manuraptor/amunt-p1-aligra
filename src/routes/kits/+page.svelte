
<script>
    import KitCard from "$lib/componentes/KitCard.svelte";




    const kits = [
        {
            title: 'KIT 1 DAMPLIACIÓ DE VOLUM',
            link: '/kitPage1',
        },
        {
            title: 'KIT 2 D’ENVOLUPANT BIOCLIMÀTICA.',
            link: '/kitPage2',
        },
        {
            title: 'KIT 3 ALJUB',
            link: '/kitPage3',
        },
        {
            title: 'KIT 4 FOTOVOLTAIC',
            link: '/kitPage4',
        },
        {
            title: 'KIT 5 SMART BUILDING',
            link: '/kitPage5',
        },
    ];




</script>

<main>
     {#each kits as kit}

         <KitCard title={kit.title} link={kit.link} />
     {/each}

</main>

<style>
    main {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 20px;
        padding: 1em;
    }
</style>
