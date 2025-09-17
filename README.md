# PORTAL-ATENDIMENTO2
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portal de Atendimento Municipal</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    /* Reset */
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: "Segoe UI", Arial, sans-serif;
      background: #f4f7fb;
      color: #333;
      line-height: 1.6;
    }

    header {
      background: #004aad;
      color: white;
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }

    header h1 {
      font-size: 2.2rem;
      margin-bottom: 5px;
    }

    header p {
      font-size: 1.1rem;
      opacity: 0.9;
    }

    nav {
      background: #036;
      display: flex;
      justify-content: center;
      gap: 30px;
      padding: 12px;
      flex-wrap: wrap;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    nav a:hover {
      color: #ffcc00;
    }

    section {
      padding: 40px 20px;
      max-width: 1100px;
      margin: auto;
    }

    h2 {
      color: #004aad;
      margin-bottom: 20px;
      border-left: 5px solid #004aad;
      padding-left: 10px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
    }

    .card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 3px 6px rgba(0,0,0,0.1);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card h3 {
      margin-bottom: 10px;
      color: #036;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    input, textarea, button {
      padding: 12px;
      font-size: 15px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }

    input:focus, textarea:focus {
      outline: none;
      border-color: #004aad;
      box-shadow: 0 0 5px rgba(0,74,173,0.3);
    }

    button {
      background: #004aad;
      color: white;
      border: none;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
    }

    button:hover {
      background: #036;
    }

    footer {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 30px;
    }

    footer p {
      font-size: 14px;
    }
  </style>
</head>
<body>
  <header>
    <h1><i class="fa-solid fa-city"></i> Prefeitura Municipal</h1>
    <p>Portal Oficial de Atendimento ao Cidadão</p>
  </header>

  <nav>
    <a href="#servicos"><i class="fa-solid fa-list"></i> Serviços</a>
    <a href="#atendimento"><i class="fa-solid fa-headset"></i> Atendimento</a>
    <a href="#contato"><i class="fa-solid fa-envelope"></i> Contato</a>
    <a href="#sobre"><i class="fa-solid fa-circle-info"></i> Sobre</a>
  </nav>

  <section id="servicos">
    <h2>Serviços Disponíveis</h2>
    <div class="grid">
      <div class="card">
        <h3><i class="fa-solid fa-calendar-check"></i> Agendamento</h3>
        <p>Solicite atendimento presencial de forma rápida e organizada.</p>
      </div>
      <div class="card">
        <h3><i class="fa-solid fa-file-signature"></i> Protocolos Online</h3>
        <p>Envie e acompanhe processos sem sair de casa.</p>
      </div>
      <div class="card">
        <h3><i class="fa-solid fa-lightbulb"></i> Sugestões</h3>
        <p>Envie ideias e propostas para melhorias na cidade.</p>
      </div>
    </div>
  </section>

  <section id="atendimento">
    <h2>Atendimento Online</h2>
    <div class="card">
      <form action="mailto:atendimento@prefeitura.gov.br" method="post" enctype="text/plain">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" name="nome" placeholder="Digite seu nome completo" required>

        <label for="email">E-mail:</label>
        <input type="email" id="email" name="email" placeholder="exemplo@email.com" required>

        <label for="mensagem">Mensagem:</label>
        <textarea id="mensagem" name="mensagem" rows="6" placeholder="Escreva sua solicitação..." required></textarea>

        <button type="submit"><i class="fa-solid fa-paper-plane"></i> Enviar Solicitação</button>
      </form>
      <p style="font-size: 13px; color: gray; margin-top: 10px;">
        ⚠️ As respostas serão enviadas para o e-mail informado.
      </p>
    </div>
  </section>

  <section id="contato">
    <h2>Contato</h2>
    <p><i class="fa-solid fa-envelope"></i> Email: atendimento@prefeitura.gov.br</p>
    <p><i class="fa-solid fa-phone"></i> Telefone: (43) 3333-0000</p>
    <p><i class="fa-solid fa-location-dot"></i> Endereço: Rua Central, 123 - Centro</p>
  </section>

  <section id="sobre">
    <h2>Sobre</h2>
    <p>Este portal foi criado para facilitar o acesso da população aos serviços municipais,
       trazendo mais agilidade, transparência e praticidade no relacionamento entre governo e cidadãos.</p>
  </section>

  <footer>
    <p>&copy; 2025 Prefeitura Municipal - Todos os direitos reservados</p>
  </footer>
</body>
</html>
