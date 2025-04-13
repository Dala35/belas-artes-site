<!DOCTYPE html>
<html lang="pt">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <meta name="description" content="Centro de Formação Profissional Belas Artes – Dança, Música, Teatro e Artes Plásticas em Angola."/>
  <title>Centro Belas Artes</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * { box-sizing: border-box; scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: #f8f8f8;
      color: #333;
    }
    header {
      background: linear-gradient(to right, #a0041e, #f5af19);
      color: white;
      text-align: center;
      padding: 30px 20px;
    }
    nav {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 15px;
      background: #fff;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      padding: 12px;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    nav a {
      text-decoration: none;
      color: #a0041e;
      font-weight: bold;
    }
    section {
      max-width: 1100px;
      margin: auto;
      padding: 30px 20px;
    }
    .highlight {
      background: #fff;
      padding: 25px;
      border-radius: 12px;
      margin-bottom: 25px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.05);
    }
    h2 { color: #a0041e; }
    iframe {
      width: 100%;
      height: 300px;
      border: none;
      border-radius: 10px;
    }
    input, select, button, textarea {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      margin-bottom: 15px;
      border-radius: 8px;
      border: 1px solid #ccc;
      font-family: 'Inter', sans-serif;
    }
    button {
      background: #a0041e;
      color: #fff;
      font-weight: bold;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background: #800317;
    }
    footer {
      background: #a0041e;
      color: white;
      text-align: center;
      padding: 20px;
      margin-top: 40px;
    }
  </style>
</head>
<body>
<header>
  <h1>Centro de Formação Profissional Belas Artes</h1>
  <p>Transformando talentos em carreiras com arte e cultura</p>
</header>

<nav>
  <a href="#cursos">Cursos</a>
  <a href="#galeria">Galeria</a>
  <a href="#blog">Blog</a>
  <a href="#eventos">Eventos</a>
  <a href="#equipa">Equipe</a>
  <a href="#mural">Mural</a>
  <a href="#inscricao">Inscrição</a>
  <a href="#contato">Contato</a>
</nav>

<section>
  <div class="highlight" id="cursos">
    <h2>Cursos em Destaque</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px;">
      <div style="background: #fafafa; padding: 15px; border-radius: 10px;">
        <h3>Dança Contemporânea</h3>
        <p>Expressão corporal e técnica com foco na criação coreográfica moderna.</p>
      </div>
      <div style="background: #fafafa; padding: 15px; border-radius: 10px;">
        <h3>Música – Canto & Instrumentos</h3>
        <p>Aulas práticas e teóricas com professores especializados em vários estilos.</p>
      </div>
      <div style="background: #fafafa; padding: 15px; border-radius: 10px;">
        <h3>Teatro</h3>
        <p>Formação em atuação e direção, com apresentações públicas e orientação artística.</p>
      </div>
      <div style="background: #fafafa; padding: 15px; border-radius: 10px;">
        <h3>Artes Visuais</h3>
        <p>Desenho, pintura e técnicas de expressão visual para artistas em formação.</p>
      </div>
    </div>
  </div>

  <div class="highlight" id="galeria">
    <h2>Galeria Interativa de Fotos e Vídeos</h2>
    <div id="galeria-conteudo" style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
      <div>
        <img src="https://source.unsplash.com/400x300/?dance" alt="Imagem inicial" style="width: 100%; border-radius: 10px;">
        <p style="text-align: center;">Apresentação artística</p>
      </div>
      <div>
        <iframe src="https://www.youtube.com/embed/ScMzIvxBSi4" title="Vídeo Apresentação" allowfullscreen></iframe>
        <p style="text-align: center;">Vídeo institucional</p>
      </div>
    </div>
    <br>
    <button onclick="acessarGaleriaAdmin()">Sou Administrador</button>
    <div id="formulario-galeria" style="display: none; margin-top: 20px;">
      <input type="text" id="linkGaleria" placeholder="Cole o link da imagem ou vídeo (ex: https://...)" />
      <button onclick="adicionarGaleria()">Adicionar à Galeria</button>
    </div>
  </div>
<div class="highlight" id="blog">
    <h2>Blog & Notícias</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px;">
      <div style="border: 1px solid #eee; border-radius: 10px; padding: 15px; background: #fafafa;">
        <h3>Nova Turma de Dança Contemporânea</h3>
        <p><strong>Data:</strong> 10 de Abril de 2025</p>
        <p>Inscrições abertas! 3 meses de formação com espetáculos de encerramento.</p>
        <button onclick="alert('Mais detalhes em breve!')">Ler mais</button>
      </div>
      <div style="border: 1px solid #eee; border-radius: 10px; padding: 15px; background: #fafafa;">
        <h3>Belas Artes no Festival Cultural</h3>
        <p><strong>Data:</strong> 25 de Março de 2025</p>
        <p>O centro participou com teatro, música e pintura ao vivo.</p>
        <button onclick="alert('Mais detalhes em breve!')">Ler mais</button>
      </div>
    </div>
  </div>

  <div class="highlight" id="eventos">
  <h2>Eventos Culturais</h2>
  <div style="display: flex; flex-direction: column; gap: 20px;">
    
    <div style="background: #fafafa; border-left: 5px solid #a0041e; padding: 15px 20px; border-radius: 8px;">
      <h3 style="margin-bottom: 5px;">Espetáculo de Teatro – “Cores da Tradição”</h3>
      <p><strong>Data:</strong> 30 de Abril de 2025</p>
      <p>Apresentação final dos alunos de Teatro com contos angolanos e direção moderna.</p>
    </div>

    <div style="background: #fafafa; border-left: 5px solid #a0041e; padding: 15px 20px; border-radius: 8px;">
      <h3 style="margin-bottom: 5px;">Exposição de Artes Visuais</h3>
      <p><strong>Data:</strong> 15 de Maio de 2025</p>
      <p>Obras dos alunos de Artes Plásticas abertas ao público em galeria temática.</p>
    </div>

    <div style="background: #fafafa; border-left: 5px solid #a0041e; padding: 15px 20px; border-radius: 8px;">
      <h3 style="margin-bottom: 5px;">Festival Belas Artes</h3>
      <p><strong>Data:</strong> 10 de Junho de 2025</p>
      <p>Um dia com dança, música, performances e feira de talentos artísticos.</p>
    </div>

  </div>
  </div>
    </div>
  </div>

  <div class="highlight" id="equipa">
  <h2>Equipe Pedagógica & Direção</h2>
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 20px;">

    <div style="text-align: center;">
      <img src="https://source.unsplash.com/150x150/?man,teacher" alt="Diretor Pedagógico" style="border-radius: 50%; width: 100px; height: 100px; object-fit: cover;">
      <h4 style="margin: 10px 0 5px;">Dala De Carvalho</h4>
      <p style="font-size: 0.9em;">Diretor Pedagógico | Educador Musical</p>
    </div>

    <div style="text-align: center;">
      <img src="https://source.unsplash.com/150x150/?woman,teacher" alt="Professora de Dança" style="border-radius: 50%; width: 100px; height: 100px; object-fit: cover;">
      <h4 style="margin: 10px 0 5px;">Helena Soares</h4>
      <p style="font-size: 0.9em;">Professora de Dança Contemporânea</p>
    </div>

    <div style="text-align: center;">
      <img src="https://source.unsplash.com/150x150/?musician" alt="Professor de Música" style="border-radius: 50%; width: 100px; height: 100px; object-fit: cover;">
      <h4 style="margin: 10px 0 5px;">Carlos André</h4>
      <p style="font-size: 0.9em;">Professor de Canto & Instrumentos</p>
    </div>

    <div style="text-align: center;">
      <img src="https://source.unsplash.com/150x150/?artist" alt="Professor de Artes" style="border-radius: 50%; width: 100px; height: 100px; object-fit: cover;">
      <h4 style="margin: 10px 0 5px;">Sandra Kiala</h4>
      <p style="font-size: 0.9em;">Professora de Pintura e Desenho</p>
    </div>

  </div>
  </div>
      </div>
    </div>
  </div>

  <div class="highlight" id="mural">
  <h2>Mural de Novidades</h2>
  <ul id="lista-mural">
    <li>Inscrições abertas para o curso de Teatro!</li>
    <li>Show de talentos no próximo sábado às 18h.</li>
  </ul>
  <br>
  <button onclick="acessarMuralAdmin()">Sou Administrador</button>
  <div id="formulario-mural" style="display: none; margin-top: 20px;">
    <input type="text" id="novo-item" placeholder="Escreva uma novidade..." />
    <button onclick="adicionarItemMural()">Adicionar ao Mural</button>
  </div>
  </div>
  </div>

  <div class="highlight" id="inscricao">
    <h2>Inscreva-se Agora</h2>
    <form onsubmit="return enviarFormulario();">
      <label for="nome">Nome:</label>
      <input type="text" id="nome" name="nome" required>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required>

      <label for="curso">Curso de Interesse:</label>
      <select id="curso" name="curso" required>
        <option value="">Selecione</option>
        <option>Dança Contemporânea</option>
        <option>Música – Canto & Instrumentos</option>
        <option>Teatro</option>
        <option>Artes Visuais</option>
      </select>

      <button type="submit">Enviar Inscrição</button>
    </form>
  </div>

  <div class="highlight" id="contato">
  <h2>Contato</h2>
  <p>Email: <a href="mailto:contato@belasartes.co.ao">contato@belasartes.co.ao</a></p>
  <p>WhatsApp: <a href="https://wa.me/244999999999" target="_blank">+244 999 999 999</a></p>
  <p>Endereço: Cuito - Bié, Angola</p>

  <h3>Localização (Em breve)</h3>
  <div style="background: #eee; padding: 15px; border-radius: 10px; text-align: center;">
    <em>Mapa será adicionado aqui futuramente com integração ao Google Maps.</em>
  </div>
  </div>
</section>

<footer>
  <p>&copy; 2025 Centro de Formação Profissional Belas Artes</p>
  <div style="margin-top: 10px;">
    <a href="https://facebook.com" target="_blank">Facebook</a> |
    <a href="https://instagram.com" target="_blank">Instagram</a> |
    <a href="https://youtube.com" target="_blank">YouTube</a>
  </div>
</footer>

<script>
  let galeriaAdmin = false;
  function acessarGaleriaAdmin() {
    const senha = prompt("Digite a senha do administrador:");
    if (senha === "belas2025") {
      galeriaAdmin = true;
      document.getElementById('formulario-galeria').style.display = "block";
    } else { alert("Senha incorreta."); }
  }
  function adicionarGaleria() {
    if (!galeriaAdmin) return;
    const link = document.getElementById('linkGaleria').value.trim();
    const container = document.createElement('div');
    if (link.includes("youtube.com/embed/")) {
      const iframe = document.createElement('iframe');
      iframe.src = link;
      iframe.width = "100%"; iframe.height = "200"; iframe.style.borderRadius = "10px";
      iframe.allowFullscreen = true;
      container.appendChild(iframe);
    } else if (link.match(/\.(jpeg|jpg|png|webp)$/)) {
      const img = document.createElement('img');
      img.src = link;
      img.style.width = "100%"; img.style.borderRadius = "10px";
      container.appendChild(img);
    } else {
      alert("Formato inválido.");
      return;
    }
    document.getElementById('galeria-conteudo').appendChild(container);
    document.getElementById('linkGaleria').value = '';
  }

  let muralAdmin = false;
  function acessarMuralAdmin() {
    const senha = prompt("Digite a senha do administrador:");
    if (senha === "belas2025") {
      muralAdmin = true;
      document.getElementById('formulario-mural').style.display = "block";
    } else {
      alert("Senha incorreta.");
    }
  }

  function adicionarItemMural() {
    if (!muralAdmin) return;
    const item = document.getElementById('novo-item').value.trim();
    if (item !== '') {
      const li = document.createElement('li');
      li.textContent = item;
      document.getElementById('lista-mural').appendChild(li);
      document.getElementById('novo-item').value = '';
    }
  }

  function enviarFormulario() {
    alert("Inscrição enviada com sucesso!");
    return false;
  }
</script>

</body>
</html>
