<script>
    export let kit;
    export let numero;

    let showModal = false;
    function openModal(){
        showModal = true;
    }
    function closeModal(){
        showModal = false;
    }


</script>

<div class="kit_card">
    <img src={kit.image} alt={kit.title}/>
    <h3>{`kit ${numero+1}: ${kit.title}`}</h3>
    <button on:click={openModal}>Leer más</button>

    {#if showModal}
        <div class="modal">
            <div class="modal-content">
                {#each kit.description as parrafo}
                    <p>{parrafo}</p>
                {/each}
                <button on:click={closeModal}>Cerrar</button>

            </div>
        </div>
    {/if}
</div>
<style>

    .kit_card {

        background-color: #f5f5f5;
        border-radius: 8px;
        padding: 1px;
        text-align: center;

    }

    img {
        width: 100%;
        object-fit: cover;
        border-radius: 8px;
        margin-bottom: 10px;
    }

    h3 {
        font-size: 18px;
        margin-bottom: 10px;


    }
    button {
        background-color: gainsboro;
        color: black;
        border: none;
        border-radius: 4px;
        padding: 10px 10px;
        font-size: 14px;
        cursor: pointer;
        margin-bottom: 5px;
    }

    p {

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