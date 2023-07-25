<script>
    export let title;
    export let link;
    export let image
</script>

<div class="KitCard">
    <h3>{title}</h3>
    <img src={image} alt="kit 1"/>
    <a href={link}>Ver más</a>
</div>

<style>
    .KitCard {
        background-color: #f5f5f5;
        border: 1px solid #ccc;
        padding: 1rem;
        margin: 1rem;
        border-radius: 8px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
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
    }


    a {
        color: black;
        text-decoration: none;

    }

    img {
        width: 100%;
        object-fit: cover;
        border-radius: 8px;
        margin-top: 90px;
    }

</style>