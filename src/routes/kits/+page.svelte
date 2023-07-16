<script>
    import KitCard from '$lib/componentes/KitCard.svelte';

    let kits = [
        {
            id: 1,
            image: 'src/lib/imagenes/kits/ImgKit1.jpg',
            title: 'KIT 1 ',
            description: 'D’AMPLIACIÓ DE VOLUM'
        },
        {
            id: 2,
            image: 'src/lib/imagenes/kits/ImgKit2.jpg',
            title: 'Kit 2',
            description: ' D’ENVOLUPANT BIOCLIMÀTICA'
        },
        {
            id: 3,
            image: 'src/lib/imagenes/kits/ImgKit3.jpg',
            title: 'KIT 3',
            description: 'KIT ALIJUB'
        },
        {
            id: 4,
            image: 'src/lib/imagenes/kits/ImgKit4.jpg',
            title: 'KIT 4',
            description: 'KIT FOTOVOLTAIC'
        },
        {
            id: 5,
            image: 'src/lib/imagenes/kits/ImgKit5.jpg',
            title: 'Kit 5',
            description: 'KIT SMART BULDING'
        }
    ];
</script>
<main>
    <div>
        {#each kits as kit (kit.id)}
            <KitCard {kit} />
        {/each}
    </div>
</main>

<style>

    div{
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        margin-left: 220px;
    }
</style>
