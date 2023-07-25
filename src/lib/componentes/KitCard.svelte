
<script>
    export let title;
    export let link;
</script>

<div class="KitCard">
    <h3>{title}</h3>
    <a href={link}>Ver más</a>
</div>

<style>
    .KitCard {
        border: 1px solid #ccc;
        padding: 1rem;
        margin: 1rem;
        border-radius: 8px;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    h3 {
        margin-bottom: 0.5rem;
    }

    a {
        color: blue;
        text-decoration: none;
    }
</style>
