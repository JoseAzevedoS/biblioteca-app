<script lang="ts">
    const Ano = new Date().getFullYear();
</script>

<div class = "footer">
    <p> &copy;
        {Ano}; Biblioteca. Todos os direitos reservados</p>
    <div class = "links">
        <a href="https://web.telegram.org/k/">Nosso Telegram</a>
        <a href="https://www.instagram.com/">Nosso Instagram</a>
        <a href="https://www.whatsapp.com/?lang=pt_BR">Nosso Whatsapp</a>
    </div>
</div>

    <style>
    .footer {
        bottom: 0;
        left: 0;
        width: 100%;
        background-color: #5c3c21;
        color: white;
        padding: 1rem;
        text-align: center;
        z-index: 1000;
    }

    .links {
        margin-top: 0.5rem;
    }

    .links a {
        color: white; 
        margin: 0 10px;
        text-decoration: none;
    }

    .links a:hover {
        text-decoration: underline;
    }
</style>