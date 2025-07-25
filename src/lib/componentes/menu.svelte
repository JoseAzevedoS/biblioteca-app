<script lang="ts">
	import Livro from './Livro.svelte';

	let livros = [
		{
			titulo: 'O Nome do Vento',
			autor: 'Patrick Rothfuss',
            foto: 'https://m.media-amazon.com/images/I/51NiIHPz4wL._SY445_SX342_.jpg'
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
        },
	];
    let livros2 = [
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
    let livros3 = [
		{ 
            titulo: 'As Crônicas de Nárnia', 
           	autor: 'C.S Lewis',
             foto: 'https://i.pinimg.com/1200x/b3/55/a7/b355a7b3293da9e6639b5ae58b5428d3.jpg'
        },
		{ 
            titulo: 'Coraline',
           	autor: 'Nail Gaiman',
             foto: 'https://i.pinimg.com/1200x/ac/6a/cc/ac6acca3e94e308e2906b1bdb3e93922.jpg'
        },
        { 
            titulo: 'A culpa é das estrelas ', 
           	autor: 'Jhon Green',
             foto: 'https://i.pinimg.com/736x/4d/cc/d8/4dccd859106a58897618f37b9ae6cd8c.jpg'
        },
        { 
            titulo: 'A Seleção', 
           	autor: 'Kiera Cass',
             foto: 'https://i.pinimg.com/736x/67/67/b4/6767b445cfeb32d39f9b0c0c2ffa20db.jpg'
        },
{ 
            titulo: 'Jogos Vorazes', 
           	autor: 'Suzanne Collins',
             foto: 'https://a-static.mlcdn.com.br/800x560/livro-jogos-vorazes/magazineluiza/234870000/b02c2f02bc79b53b0efc3dfec0fd99f6.jpg'
        }
	];
</script>

<main>
	<section class="catalogo">
		<h2>Sessão 1</h2>
		<div class="carrossel">
			{#each livros as livro}
				<Livro titulo={livro.titulo} autor={livro.autor} foto={livro.foto}/>
			{/each}
		</div>
	</section>
	<section class="catalogo">
		<h2>Sessão 2</h2>
		<div class="carrossel">
			{#each livros2 as livro}
				<Livro titulo={livro.titulo} autor={livro.autor} foto={livro.foto}/>
			{/each}
		</div>
	</section>
	<section class="catalogo">
		<h2>Sessão 3</h2>
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