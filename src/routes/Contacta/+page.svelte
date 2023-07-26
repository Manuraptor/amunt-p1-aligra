<script>
    function handleSubmit(event) {

        event.preventDefault();

        // Muestro el mensaje de exito
        const successMessage = document.querySelector('.success-message');
        successMessage.style.display = 'block';

        // Oculto el formulario
        const contactForm = document.getElementById('contact-form');
        contactForm.style.display = 'none';
    }
</script>

<main style="height: 70vh;">
    <section>
        <article>
            <h2>Contacta amb</h2>
            <h2>
                <span class="rotate-letter">A</span>
                <span class="rotate-letter">L</span>
                <span class="rotate-letter">I</span>
                <span class="rotate-letter">G</span>
                <span class="rotate-letter">R</span>
                <span class="rotate-letter">A</span>
            </h2>
        </article>
        <div class="contact-form">
            <form id="contact-form" on:submit|preventDefault={handleSubmit}>
                <div>
                    <label for="nombre">Nom complet:</label>
                    <input type="text" id="nombre" name="nombre" required />
                </div>
                <div>
                    <label for="telefono">Teléfon:</label>
                    <input type="tel" id="telefono" name="telefono" pattern="[0-9]+" required />
                </div>
                <div>
                    <label for="asunto">Assumpte:</label>
                    <input type="text" id="asunto" name="asunto" required />
                </div>
                <div>
                    <label for="mensaje">Missatge:</label>
                    <textarea id="mensaje" name="mensaje" rows="4" required></textarea>
                </div>
                <button type="submit">Enviar</button>
            </form>
        </div>
        <footer class="success-message" style="display: none;">
            El formulari ha estat enviat correctament! Aviat us respondrem.
        </footer>
    </section>


</main>

<style>
    main {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        overflow: hidden;
    }

    section {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 90%;
        padding: 20px;
        border: 1px solid #131111;
        border-radius: 10px;
    }

    article {
        width: 300px;
        text-align: center;
        margin-bottom: 90px;
    }

    .contact-form {
        width: 50%;
    }

    div {
        margin-bottom: 20px;
    }

    label {
        display: block;
        margin-bottom: 5px;
    }

    input,
    textarea {
        width: 100%;
        padding: 10px;
        border: 1px solid #ccc;
        border-radius: 5px;
        font-size: 16px;
        background-color: #f5f5f5;
    }

    textarea {
        resize: vertical;
    }

    button {
        background-color: #f5f5f5;
        color: black;
        border: 1px solid #f5f5f5;
        border-radius: 5px;
        padding: 10px 20px;
        cursor: pointer;
        font-size: 16px;
    }

    .rotate-letter {
        margin-top: 30px;
        display: inline-block;
        animation: rotateLetter 6s linear infinite;
        font-family: Impact, sans-serif;
        font-weight: lighter;
        color: #FCB900;
        font-size: 40px;
        transform-style: preserve-3d;
        perspective: 1000px;
        opacity: 0;
        animation: fadeInOut 6s linear infinite;
    }

    @keyframes rotateLetter {
        0% {
            transform: rotateX(0deg) rotateY(0deg);
        }
        100% {
            transform: rotateX(360deg) rotateY(360deg);
        }
    }

    @keyframes fadeInOut {
        0%, 100% {
            opacity: 0;
        }
        50% {
            opacity: 1;
        }
    }
    .success-message{
        margin-left: 30px;
    }

</style>
