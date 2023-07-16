<!--<script>
    import { createEventDispatcher } from 'svelte';

    export let kit;

    const dispatch = createEventDispatcher();
    let showModal = false;

    function openModal() {
        showModal = true;
    }

    function closeModal() {
        showModal = false;
    }
</script>

<div class="kit-card">
    <img src={kit.image} alt={kit.title} />
    <h3>{kit.title}</h3>
    <p>{kit.description}</p>
    <button on:click={openModal}>Leer más</button>

    {#if showModal}
        <div class="modal">
            <div class="modal-content">
                <p>Texto completo del Kit...</p>
                <button on:click={closeModal}>Cerrar</button>
            </div>
        </div>
    {/if}
</div>

<style>
    .kit-card {
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 16px;
        text-align: center;
    }

    img {
        width: 100%;
        max-height: 200px;
        object-fit: cover;
        border-radius: 8px;
        margin-bottom: 8px;
    }

    h3 {
        font-size: 20px;
        margin-bottom: 8px;
    }

    p {
        font-size: 16px;
        color: #555;
    }

    .modal {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .modal-content {
        background-color: #fff;
        border-radius: 8px;
        padding: 16px;
        max-width: 400px;
    }
</style>-->
<script>
    export let kit;
    let showModal = false;

    function openModal() {
        showModal = true;
    }

    function closeModal() {
        showModal = false;
    }
</script>

<div class="kit-card">
    <img src={kit.image} alt={kit.title} />
    <h3>{kit.title}</h3>
    <p>{kit.description}</p>
    <button on:click={openModal}>Leer más</button>

    {#if showModal}
        <div class="modal">
            <div class="modal-content">
                <p>Texto completo del Kit...</p>
                <button on:click={closeModal}>Cerrar</button>

            </div>
        </div>
    {/if}
</div>

<style>
    .kit-card {
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 16px;
        text-align: center;
    }

    img {
        width: 100%;
        max-height: 200px;
        object-fit: cover;
        border-radius: 8px;
        margin-bottom: 8px;
    }

    h3 {
        font-size: 20px;
        margin-bottom: 8px;
    }

    p {
        font-size: 16px;
        color: #555;
    }

    .modal {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.5);
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .modal-content {
        background-color: #fff;
        border-radius: 8px;
        padding: 16px;
        max-width: 400px;
    }
</style>
