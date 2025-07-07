<header class="cabecalho">
	<div class="cabecalho-principal">
		<div class="container">
			<div class="logo-area">
				<a href="index.html">
					<img
						src=""
						alt="Biblioteca - Conhecimento para Todos"
						class="logo"
					/>
				</a>
			</div>

			<div class="busca-area">
				<form action="/busca" method="get" class="form-busca">
					<input
						type="text"
						name="termo"
						placeholder="Buscar livros, autores, artigos..."
						aria-label="Campo de busca"
					/>
					<select name="categoria">
						<option value="todos">Todos</option>
						<option value="livros">Livros</option>
						<option value="autores">Autores</option>
						<option value="periodicos">Periódicos</option>
					</select>
					<button type="submit" class="botao-busca">Buscar</button>
				</form>
			</div>

			<div class="menu-icones">
				<a href="#" class="icone-link" aria-label="Minha conta">
					<i class="icone-conta"></i>
				</a>
				<a href="#" class="icone-link" aria-label="Meus empréstimos">
					<i class="icone-emprestimos"></i>
				</a>
				<a href="#" class="icone-link" aria-label="Favoritos">
					<i class="icone-favoritos"></i>
				</a>
			</div>
		</div>
	</div>

	<nav class="menu-principal">
		<div class="container">
			<ul class="menu-lista">
				<li><a href="index.html">Início</a></li>
				<li class="menu-dropdown">
					<a href="acervo.html">Acervo</a>
					<ul class="submenu">
						<li><a href="livros.html">Livros</a></li>
						<li><a href="revistas.html">Revistas</a></li>
						<li><a href="teses.html">Teses e Dissertações</a></li>
						<li><a href="multimidia.html">Multimídia</a></li>
					</ul>
				</li>
				<li><a href="servicos.html">Serviços</a></li>
				<li><a href="eventos.html">Eventos</a></li>
				<li><a href="sobre.html">Sobre a Biblioteca</a></li>
				<li><a href="contato.html">Contato</a></li>
			</ul>
		</div>
	</nav>
</header>