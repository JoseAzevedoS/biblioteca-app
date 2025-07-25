<!--<script lang="ts">
    let livros = [
        {
            id: 1,
            titulo: 'Destaque 1',
            imagem: 'https://siabi.ifrn.edu.br/instituicao/capas_destaques/47206&#39;',
            destaque: true
        },
        {
            id: 1,
            titulo: 'Diario de um banana',
            imagem: 'https://siabi.ifrn.edu.br/instituicao/capas_destaques/47391&#39;',
        }
    ];
</script>

<div class="destaque">
    <h1>Destaques</h1>
    <div class="livros flex flex-row justify-around">
        {#each livros as livro}
            {#if livro.destaque}
                <img width="150px" src={livro.imagem} alt={livro.titulo}>
            {/if}
        {/each}
    </div>
</div>

<div class="acervo">
   
</div>
-->

<script>
    import Menu from "$lib/componentes/menu.svelte";
</script>
<Menu></Menu>