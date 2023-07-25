
<script>
    import KitCard from "$lib/componentes/KitCard.svelte";




    const kits = [
        {
            title: 'KIT 1',
            link: '/kitPage1',
        },
        {
            title: 'KIT 2 ',
            link: '/kitPage2',
        },
        {
            title: 'KIT 3 ',
            link: '/kitPage3',
        },
        {
            title: 'KIT 4 ',
            link: '/kitPage4',
        },
        {
            title: 'KIT 5',
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
        grid-template-columns: repeat(5, 1fr);
        gap: 20px;
        padding: 1em;
        grid-template-rows: repeat(5, 200%);
    }
</style>
