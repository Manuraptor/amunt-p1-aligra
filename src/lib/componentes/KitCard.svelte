<script>
    export let kit;

    let showModal = false;
    function openModal(){
        showModal = true;
    }
    function closeModal(){
        showModal = false;
    }


</script>

<div class="kit-card>">
    <img src={kit.image} alt={kit.title}/>
    <h3>{kit.title}</h3>
    <p>{kit.description}</p>
    <button on:click={openModal}>Leer más</button>

    {#if showModal}
        <div class="modal">
            <div class="modal-content">
                <p>D’AMPLIACIÓ DE VOLUM<br>
                    Modularitat adaptable.<br>
                    Es tracta d'un sistema modular bidimensional,<br>
                    lleuger i en sec, desmuntable i reutilitzable, basat principalment en fusta microlaminada.<br>
                    La modulació proposada permet resoldre fàcilment diverses mides d'ampliació.<br>
                    Economia material.<br>
                    El sistema es diferencia d'altres solucions basades en fusta per la reducció<br>
                    de l’ús de material, en un exercici d'optimització radical dels recursos mitjançant l'aprofitament<br>
                    de les tècniques més avançades de la indústria de la fusta.<br>
                    Prestacions estructurals i acústiques.<br>
                    La combinació d'un entramat lleuger de fusta amb una capa de compressió de formigó armat<br>
                    colꞏlaborant permet millorar alhora les prestacions estructurals i acústiques del mòdul de forjat.
                </p>
                <button on:clik={closeModal}>Cerrar</button>

            </div>
        </div>
    {/if}
</div>
<style>

    /* .Kit-card {
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 16px;
        text-align: center;
    }

     */

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