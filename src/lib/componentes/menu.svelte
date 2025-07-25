<main>
	<section class="catalogo">
		<h2>Sessão 1</h2>

		<div class="carrossel">
			<div class="livro">
				<img src="" alt="Livro 1" />
				<h3>O Nome do Vento</h3>
				<p>Patrick Rothfuss</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 2" />
				<h3>Dom Casmurro</h3>
				<p>Machado de Assis</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 3" />
				<h3>1984</h3>
				<p>George Orwell</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 4" />
				<h3>1999</h3>
				<p>Mayra</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 4" />
				<h3>1999</h3>
				<p>Mayra</p>
			</div>
		</div>
	</section>
	<section class="catalogo">
		<h2>Sessão 2</h2>
		<div class="carrossel">
			<div class="livro">
				<img src="" alt="Livro 5" />
				<h3>1984</h3>
				<p>George Orwell</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
		</div>
	</section>
	<section class="catalogo">
		<h2>Sessão 3</h2>
		<div class="carrossel">
			<div class="livro">
				<img src="" alt="Livro 5" />
				<h3>1984</h3>
				<p>George Orwell</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
			<div class="livro">
				<img src="" alt="Livro 6" />
				<h3>O Pequeno Príncipe</h3>
				<p>Antoine de Saint-Exupéry</p>
			</div>
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

	.livro {
		flex: 0 0 auto;
		width: 160px;
		background-color: white;
		border-radius: 8px;
		padding: 15px;
		text-align: center;
		box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
		transition:
			transform 0.3s,
			box-shadow 0.3s;
	}

	.livro:hover {
		transform: translateY(-5px);
		box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
	}

	.livro img {
		width: 100%;
		height: 220px;
		object-fit: cover;
		border-radius: 4px;
		margin-bottom: 15px;
		box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
	}

	.livro h3 {
		font-size: 16px;
		margin-bottom: 5px;
		color: var(--dark-color);
		white-space: nowrap;
		overflow: hidden;
		text-overflow: ellipsis;
	}

	.livro p {
		font-size: 14px;
		color: var(--secondary-color);
		font-style: italic;
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
