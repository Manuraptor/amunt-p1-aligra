<script>
    import KitCard from '$lib/componentes/KitCard.svelte';

    let kits = [
        {
            image: 'src/lib/imagenes/kits/ImgKit1.jpg',
            title: 'D’AMPLIACIÓ DE VOLUM',
            description: [
                "Modularitat adaptable." +
                "Es tracta d'un sistema modular bidimensional, lleuger i en sec, desmuntable i reutilitzable, basat principalment en fusta microlaminada.",
                "La modulació proposada permet resoldre fàcilment diverses mides d'ampliació.",
                "Economia material.",
                "El sistema es diferencia d'altres solucions basades en fusta per la reducció",
                "de l’ús de material, en un exercici d'optimització radical dels recursos mitjançant l'aprofitament",
                "de les tècniques més avançades de la indústria de la fusta.",
                "Prestacions estructurals i acústiques.",
                "La combinació d'un entramat lleuger de fusta amb una capa de compressió de formigó armat",
                "colꞏlaborant permet millorar alhora les prestacions estructurals i acústiques del mòdul de forjat."
            ]
        },
        {
            image: 'src/lib/imagenes/kits/ImgKit2.jpg',
            title: 'Kit 2',
            description: []
        },
        {
            image: 'src/lib/imagenes/kits/ImgKit3.jpg',
            title: 'KIT 3',
            description: []
        },
        {
            image: 'src/lib/imagenes/kits/ImgKit4.jpg',
            title: 'KIT 4',
            description: []
        },
        {
            image: 'src/lib/imagenes/kits/ImgKit5.jpg',
            title: 'Kit 5',
            description: []
        }
    ];
</script>
<main>
    <div>
        {#each kits as kit,i}
            <KitCard numero={i} {kit} />
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

