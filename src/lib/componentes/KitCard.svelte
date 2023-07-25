<script>
    export let title;
    export let link;
    export let image

</script>

<div class="KitCard">
    <h1>{title}</h1>
    <img src={image} alt="kit 1"/>
    <a href={link}>*</a>
</div>

<style>

    .KitCard {

        border: 6px solid black;
        padding: 1rem;
        margin: 0.2rem;
        border-radius: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
<<<<<<< HEAD

    }

    h1 {
        font-family: Impact, SansSerif;
        margin-bottom: 1rem;
=======
        box-shadow: 5px 5px 5px #cccccc;

    }

    .KitCard:hover {
        background-color: #FCB900;
    }

    .KitCard:hover a {

        color: white;

    }

    h3 {
        margin-bottom: 0.5rem;
>>>>>>> bff506c379325ba0d324fa22268d3236820ce74a
    }


    a {
        color: black;
        text-decoration: none;

    }

    img {
        width: 100%;
        object-fit: cover;
        border-radius: 8px;
<<<<<<< HEAD
        margin-top: 100px;
        margin-bottom: 10px;
=======
        margin-top: 90px;
>>>>>>> bff506c379325ba0d324fa22268d3236820ce74a
    }



</style>