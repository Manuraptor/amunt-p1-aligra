
<script>
    import  ImgKit1  from "$lib/imagenes/kits/ImgKit1.jpg";
    import  ImgKit2  from "$lib/imagenes/kits/ImgKit2.jpg";
    import  ImgKit3  from "$lib/imagenes/kits/ImgKit3.jpg";
    import  ImgKit4  from "$lib/imagenes/kits/ImgKit4.jpg";
    import  ImgKit5  from "$lib/imagenes/kits/ImgKit5.jpg";
    import '/src/global.css'



</script>
<main>
    <section>

        <h1>PARTS QUE LA COMPOSEN</h1>
        <div class="articulos">

            <img src={ImgKit1} alt="kits">

            <img src={ImgKit2} alt="kits">

            <img src={ImgKit3} alt="kits">

            <img src={ImgKit4} alt="kits">

            <img src={ImgKit5} alt="kits">

        </div>

    </section>
</main>
<style>
    main{
        margin-left: 160px;
    }

    h1{
        text-align: center;
        font-size: 40px;
        padding-top: 50px;
        height: 50px;
        padding: 60px;
        right: 40px;
    }

    .articulos {
        display: grid;
        grid-template-columns: repeat(2, 1fr) ;
        margin: 50px 50px;
    }

    img {
        width: 700px;
        height: 350px;
    }


</style>
