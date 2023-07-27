<script>
    export let title;
    export let link;
    export let image;
    export let subtitle

</script>

<div class="KitCard">
    <a href={link}>
    <h2>{title}</h2>
    </a>
    <h4>{subtitle}</h4>
    <img src={image} alt="kit 1"/>

</div>

<style>

    .KitCard {
        border: 4px solid black;
        padding: 1rem;
        margin: 0;
        border-radius: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-between;
        height: 500px;
    }


    h2 {
        font-family: Impact, sans-serif;
        font-size: 24px;
        margin-bottom: 1rem;
    }
    h4 {
        font-size: 12px;

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

