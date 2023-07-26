<script>
    export let title;
    export let link;
    export let image

</script>

<div class="KitCard">
    <a href={link}>
    <h2>{title}</h2>
    </a>
    <img src={image} alt="kit 1"/>

</div>

<style>

    .KitCard {
        border: 6px solid black;
        padding: 1rem;
        margin: 0;
        border-radius: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        /* Set the height to control the card's size */
        height: 500px;
    }


    h2 {
        font-family: Impact, sans-serif;
        font-size: 24px;
        margin-bottom: 1rem;
    }

    a {
        color: black;
        text-decoration: none;
    }


    img {
         width: 100%;
        object-fit: cover;
        border-radius: 8px;
        margin-bottom: 10px;
    }

</style>

