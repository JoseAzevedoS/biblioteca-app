<script lang="ts">
	import Livro from './Livro.svelte';

	let livros = [
		{
			titulo: 'Verity',
			autor: 'Colleen Hoover',
            foto: 'https://i.pinimg.com/736x/0e/20/60/0e206030a674bf384469e08aabfdf486.jpg'
		},
		{ 
            titulo: 'Tudo o que eu sei sobre o amor', 
           	autor: 'Dolly Alderton',
             foto: 'https://i.pinimg.com/736x/b9/fe/12/b9fe1276bc5124d8867de5e139f3d777.jpg'
        },
        { 
            titulo: 'Meu amigo espírito santo', 
           	autor: 'Ade Huber',
             foto: 'https://i.pinimg.com/736x/d6/67/de/d667def6f0a5e3dad9ffa75f83b612af.jpg'
        },
        { 
            titulo: 'Um sopro de vida', 
           	autor: 'Clarice Lispector',
             foto: 'https://i.pinimg.com/1200x/21/24/70/21247006e3779e7bbe1bae2b1cb1f39a.jpg'
        },
        { 
            titulo: 'Hábitos atômicos', 
           	autor: 'James Clear',
             foto: 'https://i.pinimg.com/736x/70/4c/00/704c002733b81135ebc1a90784e33c0e.jpg'
        },
	];
    let livros2 = [
		{ 
            titulo: 'Eu e Esse Meu Coração', 
           	autor: 'C. C. Hunter',
             foto: 'https://i.pinimg.com/1200x/d8/d0/d2/d8d0d25e9357d142df157723f34fea20.jpg'
        },
		{ 
            titulo: 'Ainda Ontem Pensei Com o Coração', 
           	autor: 'Vini Queiroz',
             foto: 'https://i.pinimg.com/1200x/99/5f/91/995f913fdb0ec91c7290492c93e7586b.jpg'
        },
        { 
            titulo: 'O Amor Não é Óbvio ', 
           	autor: 'Elayne Baeta',
             foto: 'https://i.pinimg.com/1200x/54/76/2e/54762e45c0efba8660f50f6370a243bf.jpg'
        },
        { 
            titulo: 'Coisas Óbvias Sobre O Amor', 
           	autor: 'Elayne Baeta',
             foto: 'https://i.pinimg.com/736x/d5/6a/b0/d56ab008d4a66f69c2119646f4e6bd25.jpg'
        },
{ 
            titulo: 'Oxe Baby', 
           	autor: 'Elayne Baeta',
             foto: 'https://i.pinimg.com/736x/39/49/46/394946478b0c808c604a5ef9db5a53b6.jpg'
        }
	];
    let livros3 = [
		{ 
            titulo: 'O temor do sábio', 
           	autor: 'Patrick Rothfuss',
             foto: 'https://m.media-amazon.com/images/I/91rGGj7JBhL._SY425_.jpg'
        },
		{ 
            titulo: 'O temor do sábio', 
           	autor: 'Patrick Rothfuss',
             foto: 'https://m.media-amazon.com/images/I/91rGGj7JBhL._SY425_.jpg'
        },
        { 
            titulo: 'O temor do sábio', 
           	autor: 'Patrick Rothfuss',
             foto: 'https://m.media-amazon.com/images/I/91rGGj7JBhL._SY425_.jpg'
        },
        { 
            titulo: 'O temor do sábio', 
           	autor: 'Patrick Rothfuss',
             foto: 'https://m.media-amazon.com/images/I/91rGGj7JBhL._SY425_.jpg'
        },
{ 
            titulo: 'O temor do sábio', 
           	autor: 'Patrick Rothfuss',
             foto: 'https://m.media-amazon.com/images/I/91rGGj7JBhL._SY425_.jpg'
        }
	];
</script>

<main>
	<section class="catalogo">
		<h2>Destaques</h2>
		<div class="carrossel">
			{#each livros as livro}
				<Livro titulo={livro.titulo} autor={livro.autor} foto={livro.foto}/>
			{/each}
		</div>
	</section>
	<section class="catalogo">
		<h2>Favoritos</h2>
		<div class="carrossel">
			{#each livros2 as livro}
				<Livro titulo={livro.titulo} autor={livro.autor} foto={livro.foto}/>
			{/each}
		</div>
	</section>
	<section class="catalogo">
		<h2>Lançamentos</h2>
		<div class="carrossel">
            {#each livros3 as livro}
				<Livro titulo={livro.titulo} autor={livro.autor} foto={livro.foto} />
			{/each}
		</div>
	</section>
</main>

<style>
	:root {
		--primary-color: #5c3c21;
		--secondary-color: #8b5a2b;
		--accent-color: #d4a76a;
		--light-color: #f5f0e6;
		--dark-color: #2c1a0d;
		--text-color: #333;
		--text-light: #f8f8f8;
	}

	* {
		margin: 0;
		padding: 0;
		box-sizing: border-box;
		font-family: 'Georgia', 'Times New Roman', serif;
	}

	body {
		background-color: var(--light-color);
		color: var(--text-color);
		line-height: 1.6;
	}

	main {
		padding: 40px 20px;
		max-width: 1200px;
		margin: 0 auto;
	}

	.catalogo {
		margin-bottom: 40px;
	}

	.catalogo h2 {
		color: var(--primary-color);
		font-size: 24px;
		margin-bottom: 20px;
		padding-bottom: 10px;
		border-bottom: 2px solid var(--accent-color);
	}

	.carrossel {
		display: flex;
		gap: 20px;
		overflow-x: auto;
		scroll-behavior: smooth;
		padding: 20px 10px;
		scrollbar-width: thin;
		scrollbar-color: var(--accent-color) var(--light-color);
	}

	.carrossel::-webkit-scrollbar {
		height: 8px;
	}

	.carrossel::-webkit-scrollbar-track {
		background: var(--light-color);
		border-radius: 4px;
	}

	.carrossel::-webkit-scrollbar-thumb {
		background-color: var(--accent-color);
		border-radius: 4px;
	}

	@media (max-width: 768px) {
		.carrossel {
			padding: 15px 5px;
		}

		.livro {
			width: 140px;
			padding: 10px;
		}

		.livro img {
			height: 180px;
		}
	}
</style>