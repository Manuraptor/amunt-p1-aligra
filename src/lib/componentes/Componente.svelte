<script>
export let imagen
export let texto


</script>

<section>
    <img src={imagen} alt="imagen">
    <p>{texto}</p>

</section>



<style>


    section{

        display: flex;
        flex-direction: row;
        justify-content: space-around;
        height: 100px;
        width: 900px;
        gap:85px;
        margin-left: 275px;
    }


</style>