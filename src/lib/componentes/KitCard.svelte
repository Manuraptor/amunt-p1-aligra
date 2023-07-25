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
        margin: 0rem;
        border-radius: 15px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;}

    h1 {
        font-family: Impact, SansSerif;
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
        margin-top: 100px;
        margin-bottom: 10px;

    }

</style>