<script>
    export let imagen
    export let texto

    export let titulo

    import {fade} from 'svelte/transition';

</script>

<section>
    <img transition:fade src={imagen} alt="logo"/>
    <h2>{titulo}</h2>
    <p>{texto}</p>

</section>


<style>


    section {

        display: flex;
        flex-direction: column;
        justify-content: space-around;
      /*  height: 100px;
        width: 900px;*/
        gap: 15px;
   /*     margin-left: 275px;*/
        margin-bottom: 60px;
        align-items: center;
    }

    img {
        width: 200px;
        filter: grayscale(100%);
        transition: all 0.5s ease;
    }

    img:hover {
        filter: none;
        transform: scale(1.1);
    }
</style>