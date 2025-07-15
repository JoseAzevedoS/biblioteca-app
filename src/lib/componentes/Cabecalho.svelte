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

.container {
    width: 100%;
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

a {
    text-decoration: none;
    color: inherit;
    transition: all 0.3s ease;
}

.cabecalho {
    background-color: var(--primary-color);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
}

.cabecalho-principal {
    padding: 15px 0;
    background-color: var(--primary-color);
    border-bottom: 3px solid var(--accent-color);
}

.logo-area {
    display: flex;
    align-items: center;
}

.logo {
    height: 60px;
    width: auto;
    filter: drop-shadow(0 2px 4px rgba(0, 0, 0, 0.2));
}

.busca-area {
    flex-grow: 1;
    margin: 0 30px;
}

.form-busca {
    display: flex;
    align-items: center;
}

.form-busca input[type="text"] {
    flex-grow: 1;
    padding: 10px 15px;
    border: 1px solid #ddd;
    border-radius: 4px 0 0 4px;
    font-size: 16px;
    background-color: var(--light-color);
    color: var(--text-color);
}

.form-busca select {
    padding: 10px;
    border: 1px solid #ddd;
    border-left: none;
    background-color: var(--light-color);
    color: var(--text-color);
    cursor: pointer;
}

.form-busca button {
    padding: 10px 20px;
    background-color: var(--secondary-color);
    color: white;
    border: none;
    border-radius: 0 4px 4px 0;
    cursor: pointer;
    font-weight: bold;
    transition: background-color 0.3s;
}

.form-busca button:hover {
    background-color: var(--dark-color);
}

.menu-icones {
    display: flex;
    align-items: center;
    gap: 20px;
}

.icone-link {
    color: var(--light-color);
    font-size: 24px;
    position: relative;
    padding: 5px;
}

.icone-link:hover {
    color: var(--accent-color);
}

.icone-link::after {
    content: attr(aria-label);
    position: absolute;
    bottom: -30px;
    left: 50%;
    transform: translateX(-50%);
    background-color: var(--dark-color);
    color: white;
    padding: 5px 10px;
    border-radius: 4px;
    font-size: 12px;
    opacity: 0;
    transition: opacity 0.3s;
    pointer-events: none;
    white-space: nowrap;
}

.icone-link:hover::after {
    opacity: 1;
}

.menu-principal {
    background-color: var(--secondary-color);
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.menu-lista {
    display: flex;
    list-style: none;
}

.menu-lista > li {
    position: relative;
}

.menu-lista > li > a {
    display: block;
    padding: 15px 20px;
    color: var(--text-light);
    font-weight: 500;
    text-transform: uppercase;
    font-size: 14px;
    letter-spacing: 0.5px;
    transition: all 0.3s;
}

.menu-lista > li > a:hover {
    background-color: var(--accent-color);
    color: var(--dark-color);
}

.menu-dropdown:hover .submenu {
    display: block;
}

.submenu {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    background-color: var(--light-color);
    min-width: 200px;
    box-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
    z-index: 100;
    border-radius: 0 0 4px 4px;
}

.submenu li {
    border-bottom: 1px solid #eee;
}

.submenu li:last-child {
    border-bottom: none;
}

.submenu a {
    display: block;
    padding: 12px 20px;
    color: var(--text-color);
    transition: all 0.3s;
}

.submenu a:hover {
    background-color: var(--accent-color);
    color: var(--dark-color);
    padding-left: 25px;
}

.cabecalho-principal .container {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

@media (max-width: 992px) {
    .cabecalho-principal .container {
        flex-direction: column;
        gap: 15px;
    }
    
    .busca-area {
        width: 100%;
        margin: 15px 0;
    }
    
    .menu-lista {
        flex-wrap: wrap;
        justify-content: center;
    }
    
    .menu-lista > li > a {
        padding: 10px 15px;
    }
}

@media (max-width: 768px) {
    .form-busca {
        flex-direction: column;
        gap: 10px;
    }
    
    .form-busca input[type="text"],
    .form-busca select,
    .form-busca button {
        width: 100%;
        border-radius: 4px;
    }
    
    .menu-lista {
        flex-direction: column;
    }
    
    .menu-dropdown:hover .submenu {
        position: static;
        box-shadow: none;
    }
}
</style>