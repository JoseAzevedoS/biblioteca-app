<main>
	<section class="catalogo">
		<h2>Sessão 1</h2>

		<div class="carrossel">
			<div class="livro">
				<img src="https://i.pinimg.com/736x/7b/61/9b/7b619b66ada89eb3620f3a18ebd255cb.jpg" alt="Livro 1" />
				<h3>Meu amigo espírito santo</h3>
				<p>Abe Huber</p>
			</div>
			<div class="livro">
				<img src="https://i.pinimg.com/736x/fb/d3/55/fbd355c889f2efbff5189b6a621bb004.jpg" alt="Livro 2" />
				<h3>Os sete maridos de Evelyn Hugo</h3>
				<p>Colleen Hoover</p>
			</div>
			<div class="livro">
				<img src="https://i.pinimg.com/736x/de/61/ea/de61eaa47714673e1f1a65c6f7cb5af0.jpg" alt="Livro 3" />
				<h3>Calma aí, porra</h3>
				<p>Sarah Knignt</p>
			</div>
			<div class="livro">
				<img src="https://i.pinimg.com/736x/b9/fe/12/b9fe1276bc5124d8867de5e139f3d777.jpg" alt="Livro 4" />
				<h3>Tudo o que eu sei sobre o amor</h3>
				<p>Dolly Alderton</p>
			</div>
			<div class="livro">
				<img src="https://i.pinimg.com/736x/0e/20/60/0e206030a674bf384469e08aabfdf486.jpg" alt="Livro 4" />
				<h3>Verity</h3>
				<p>Colleen Hoover</p>
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
