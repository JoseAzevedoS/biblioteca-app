<script lang="ts">
	const { titulo, autor,foto } = $props();
</script>

<div class="livro">
	<img src={foto} alt="Livro 1" />
	<h3>{titulo}</h3>
	<p>{autor}</p>
</div>

<style>
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
</style>
