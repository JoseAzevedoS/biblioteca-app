<head>
  <style>
    .menu-toggle {
  display: none;
}
@media (max-width: 768px) {
  .menu-toggle {
    display: block;
    font-size: 26px;
    background: none;
    border: none;
    padding: 15px;
    cursor: pointer;
    color: white;
    background-color: #333;
    width: 100%;
    text-align: left;
  }
}
    .carrossel {
      display: flex;
      gap: 20px;
      overflow-x: auto;
      scroll-behavior: smooth;
      padding: 10px;
    }

    .livro {
      flex: 0 0 auto;
      width: 160px;
      background-color: #f5f5f5;
      border-radius: 8px;
      padding: 10px;
      text-align: center;
    }

    .livro img {
      width: 100%;
      border-radius: 4px;
    }
  </style>
</head>
<body>
  <header>
    <button class="menu-toggle" id="menu-toggle">&#9776;</button>
    
    <nav class="menu" id="menu">
      <a href="index.html">Início</a>
      <a href="catalogo.html">Catálogo</a>                                                                                                           
      <a href="emprestimos.html">Empréstimos</a>
      <a href="servicos.html">Serviços</a>
      <a href="eventos.html">Eventos</a>
      <a href="contato.html">Contato</a>
      <a href="sobre.html">Sobre</a>
    </nav>
  </header>

  <main>
    <section class="catalogo">
      <h2>Sessão 1</h2>

      <div class="carrossel">
        <div class="livro">
          <img src="https://via.placeholder.com/150x220?text=Livro+1" alt="Livro 1" />
          <h3>O Nome do Vento</h3>
          <p>Patrick Rothfuss</p>
        </div>
        <div class="livro">
          <img src="https://via.placeholder.com/150x220?text=Livro+2" alt="Livro 2" />
          <h3>Dom Casmurro</h3>
          <p>Machado de Assis</p>
        </div>
        <div class="livro">
          <img src="https://via.placeholder.com/150x220?text=Livro+3" alt="Livro 3" />
          <h3>1984</h3>
          <p>George Orwell</p>
        </div>
         <div class="livro">
          <img src="https://via.placeholder.com/150x220?text=Livro+3" alt="Livro 4" />
          <h3>1999</h3>
          <p>Mayra</p>
        </div>
         <div class="livro">
          <img src="https://via.placeholder.com/150x220?text=Livro+3" alt="Livro 4" />
          <h3>1999</h3>
          <p>Mayra</p>
        </div>
      </div>
    </section>
    <section class="catalogo">
        <h2>Sessão 2</h2>
        <div class="carrossel">
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+4" alt="Livro 5" />
                <h3>1984</h3>
                <p>George Orwell</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
        </div>
    </section>
    <section class="catalogo">
        <h2>Sessão 3</h2>
        <div class="carrossel">
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+4" alt="Livro 5" />
                <h3>1984</h3>
                <p>George Orwell</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
            <div class="livro">
                <img src="https://via.placeholder.com/150x220?text=Livro+5" alt="Livro 6" />
                <h3>O Pequeno Príncipe</h3>
                <p>Antoine de Saint-Exupéry</p>
            </div>
        </div>
    </section>
  </main>

  <script src="script.js"></script>
</body>

