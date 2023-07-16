<script>
import KitCard from '$lib/componentes/KitCard.svelte';

let kits = [
{
    id: 1,
    image: 'src/lib/imagenes/kits/ImgKit1.jpg',
    title: 'Kit 1',
    description: 'Descripción del Kit 1...'
},
{
    id: 2,
    image: 'src/lib/imagenes/kits/ImgKit2.jpg',
    title: 'Kit 2',
    description: 'Descripción del Kit 2...'
},
{
    id: 3,
    image: 'src/lib/imagenes/kits/ImgKit3.jpg',
    title: 'Kit 3',
    description: 'Descripción del Kit 2...'
},
{
    id: 4,
    image: 'src/lib/imagenes/kits/ImgKit4.jpg',
    title: 'Kit 4',
    description: 'Descripción del Kit 2...'
},
{
    id: 5,
    image: 'src/lib/imagenes/kits/ImgKit5.jpg',
    title: 'Kit 5',
    description: 'Descripción del Kit 2...'
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