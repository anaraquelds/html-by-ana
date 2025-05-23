<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Guia Calouro SI 👾 IFAL Arapiraca</title>
    <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&family=Roboto:wght@300;400;700&family=Aldrich&display=swap" rel="stylesheet">
    <style>
        :root {
            --cor-fundo-dark: #12121F;
            --cor-container-dark: #1A1A2E;
            --cor-texto-principal: #E0E0E0;
            --cor-texto-secundario: #A0A0B0;
            --cor-destaque-neon-ciano: #00FFFF;
            --cor-destaque-neon-magenta: #FF00FF;
            --cor-destaque-neon-verde: #39FF14;
            --cor-ifal-azul-adapt: #2D68A2;
            --cor-ifal-verde-adapt: #38A34A;
            --sombra-neon-suave: 0 0 8px rgba(var(--rgb-destaque-neon-ciano), 0.5), 0 0 12px rgba(var(--rgb-destaque-neon-ciano), 0.3);
            --rgb-destaque-neon-ciano: 0, 255, 255;
            --fonte-pixel: 'Press Start 2P', cursive;
            --fonte-tech: 'Aldrich', sans-serif;
            --fonte-corpo: 'Roboto', sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html {
            scroll-behavior: smooth; /* Adiciona scroll suave via CSS (funciona na maioria dos navegadores modernos) */
        }

        body {
            font-family: var(--fonte-corpo);
            line-height: 1.6;
            color: var(--cor-texto-principal);
            background-color: var(--cor-fundo-dark);
            overflow-x: hidden;
            font-size: 15px;
        }

        h1, h2, h3, h4 {
            font-family: var(--fonte-tech);
            font-weight: 700;
            margin-bottom: 15px;
        }

        h1 { font-size: 1.8em; color: var(--cor-destaque-neon-ciano); text-align: center; text-shadow: 0 0 8px var(--cor-destaque-neon-ciano), 0 0 4px #fff; margin-bottom: 15px;}
        h2 { font-size: 1.6em; color: var(--cor-destaque-neon-magenta); border-bottom: 2px solid var(--cor-destaque-neon-magenta); padding-bottom: 8px; margin-top: 35px; }
        h3 { font-size: 1.3em; color: var(--cor-destaque-neon-verde); }
        h4 { font-size: 1.1em; color: var(--cor-destaque-neon-ciano); }

        p { margin-bottom: 12px; font-size: 0.95em; color: var(--cor-texto-secundario); }
        strong { color: var(--cor-texto-principal); font-weight: 700; }

        a { color: var(--cor-destaque-neon-ciano); text-decoration: none; transition: color 0.3s ease, text-shadow 0.3s ease; }
        a:hover { color: #fff; text-shadow: 0 0 8px var(--cor-destaque-neon-ciano); }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px 0;
        }

        header {
            background-color: rgba(26, 26, 46, 0.85);
            backdrop-filter: blur(10px);
            padding: 10px 0;
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 2px solid var(--cor-destaque-neon-ciano);
            box-shadow: 0 2px 10px rgba(var(--rgb-destaque-neon-ciano), 0.2);
        }

        header .container-header {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        header .logo {
            font-family: var(--fonte-pixel);
            font-size: 1em;
            color: var(--cor-destaque-neon-verde);
            text-shadow: 0 0 5px var(--cor-destaque-neon-verde);
            margin-bottom: 10px;
        }
        header .logo span { color: var(--cor-texto-principal); font-size: 0.9em;}

        nav ul {
            list-style: none;
            display: flex;
            flex-direction: column;
            align-items: center;
            width: 100%;
        }
        nav ul li {
            margin: 4px 0;
            width: 90%;
            text-align: center;
        }
        nav ul li a {
            font-family: var(--fonte-tech);
            color: var(--cor-texto-principal);
            font-size: 0.9em;
            padding: 8px 8px;
            border-radius: 4px;
            border: 1px solid transparent;
            transition: all 0.3s ease;
            display: block;
        }
        nav ul li a:hover, nav ul li a:focus { /* :focus para acessibilidade e navegação por teclado */
            color: var(--cor-fundo-dark);
            background-color: var(--cor-destaque-neon-ciano);
            border-color: var(--cor-destaque-neon-ciano);
            box-shadow: var(--sombra-neon-suave);
            text-shadow: none;
        }
        /* Para o link ativo, sem JS, teríamos que usar uma classe manual ou depender do :target */
        /* Exemplo com :target (limitado, só funciona após clique e se o ID da seção estiver na URL) */
        section:target {
           /* Você poderia adicionar um destaque sutil à seção ativa, mas não ao link do menu */
           /* border-top: 2px solid var(--cor-destaque-neon-verde); */
        }


        section {
            padding: 30px 15px;
            margin-bottom: 20px;
            background-color: var(--cor-container-dark);
            border-radius: 10px;
            border: 1px solid rgba(var(--rgb-destaque-neon-ciano), 0.15);
            box-shadow: 0 0 15px rgba(10, 10, 26, 0.4);
            position: relative;
        }

        #boas-vindas { text-align: center; background: none; box-shadow: none; border: none; padding-top: 5px; }
        #boas-vindas .lead { font-size: 1em; color: var(--cor-texto-secundario); max-width: 100%; margin: 0 auto 20px auto; }
        #boas-vindas .lead strong { color: var(--cor-destaque-neon-verde); }
        #boas-vindas .campus-info { font-family: var(--fonte-tech); font-size: 1.1em; color: var(--cor-destaque-neon-magenta); margin-top: -10px; }

        .info-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
        }
        .info-card {
            background-color: rgba(10, 10, 26, 0.7);
            padding: 20px;
            border-radius: 8px;
            border: 1px solid var(--cor-ifal-azul-adapt);
            box-shadow: 0 0 8px rgba(var(--rgb-destaque-neon-ciano), 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .info-card:hover {
            transform: translateY(-3px) scale(1.01);
            box-shadow: 0 0 12px rgba(var(--rgb-destaque-neon-ciano), 0.25);
        }
        .info-card h3 { margin-top: 0; border-bottom: 1px dashed var(--cor-destaque-neon-verde); padding-bottom: 8px;}

        .disciplinas-grid {
            display: grid;
            grid-template-columns: 1fr;
            gap: 20px;
            margin-top: 20px;
        }
        .disciplina-card {
            background-color: var(--cor-fundo-dark);
            padding: 15px;
            border-radius: 10px;
            border: 2px solid var(--cor-container-dark);
            position: relative;
            overflow: hidden;
            transition: transform 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275), box-shadow 0.4s ease;
            box-shadow: 0 4px 12px rgba(0,0,0,0.25);
        }
         .disciplina-card::before {
            content: ''; position: absolute; top: -50%; left: -50%; width: 200%; height: 200%;
            background: conic-gradient(transparent, transparent, transparent, var(--cor-destaque-neon-ciano));
            animation: rotate 4s linear infinite paused; opacity: 0; transition: opacity 0.4s ease;
        }
        .disciplina-card:hover::before { animation-play-state: running; opacity: 1; }
        .disciplina-card:hover {
            transform: translateY(-5px);
            border-color: var(--cor-destaque-neon-ciano);
            box-shadow: 0 0 20px rgba(var(--rgb-destaque-neon-ciano), 0.35), 0 8px 15px rgba(0,0,0,0.35);
        }
        .disciplina-card-content {
            position: relative; z-index: 1; background-color: var(--cor-fundo-dark);
            padding: 12px; border-radius: 8px; height: calc(100% - 24px); display: flex; flex-direction: column;
        }
        @keyframes rotate { 100% { transform: rotate(1turn); } }

        .disciplina-card .professor { font-size: 0.85em; }
        .disciplina-card .ementa-placeholder { font-size: 0.85em; flex-grow: 1; }
        .disciplina-card .tag { padding: 4px 8px; font-size: 0.7em; margin-top: 10px; }

        .info-horario-geral {
            text-align: center; font-family: var(--fonte-tech); font-size: 1em;
            color: var(--cor-texto-principal); background: linear-gradient(45deg, var(--cor-destaque-neon-ciano), var(--cor-destaque-neon-magenta));
            -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
            padding: 8px; border-radius: 5px; margin-bottom: 20px; border: 1px solid var(--cor-destaque-neon-magenta);
        }
        .info-horario-geral strong { -webkit-text-fill-color: initial; color: var(--cor-destaque-neon-verde); }

        .horario-semanal table {
            width: 100%; border-collapse: separate; border-spacing: 0;
            margin-top: 15px; font-size: 0.85em;
            border: 1px solid var(--cor-destaque-neon-magenta); border-radius: 8px; overflow: hidden;
        }
        .horario-semanal th, .horario-semanal td {
            border-bottom: 1px solid var(--cor-container-dark); padding: 10px 8px; text-align: left;
        }
        .horario-semanal th {
            background-color: var(--cor-destaque-neon-magenta); color: var(--cor-fundo-dark);
            font-family: var(--fonte-tech); font-weight: 700;
        }
        .horario-semanal td { background-color: rgba(26, 26, 46, 0.7); }
        .horario-semanal td:first-child { font-weight: bold; color: var(--cor-destaque-neon-ciano); }
        .horario-semanal tr:last-child td { border-bottom: none; }
        .horario-semanal td strong { color: var(--cor-destaque-neon-verde); }

        .nota-ead { margin-top: 12px; font-size: 0.85em; }
        .nota-ead strong { color: var(--cor-destaque-neon-verde); }

        #dicas ul { list-style: none; padding-left: 0; }
        #dicas ul li {
            background-color: rgba(10, 10, 26, 0.7); padding: 10px 15px;
            margin-bottom: 8px; border-radius: 6px; border-left: 3px solid var(--cor-destaque-neon-ciano);
            transition: background-color 0.3s ease, border-left-color 0.3s ease; font-size: 0.9em;
        }
        #dicas ul li:hover { background-color: var(--cor-container-dark); border-left-color: var(--cor-destaque-neon-verde); }
        #dicas ul li::before { content: '🎮'; margin-right: 8px; color: var(--cor-destaque-neon-ciano); }

        footer {
            text-align: center; padding: 25px 0; background-color: var(--cor-container-dark);
            color: var(--cor-texto-secundario); margin-top: 30px; font-size: 0.8em;
            border-top: 2px solid var(--cor-destaque-neon-magenta);
        }
        footer p { margin-bottom: 5px; }
        footer .ifal-logo-footer { font-family: var(--fonte-pixel); color: var(--cor-destaque-neon-verde); }

        @media (min-width: 768px) {
            body { font-size: 16px; line-height: 1.7; }
            h1 { font-size: 2.6em; margin-bottom: 20px; }
            h2 { font-size: 2em; padding-bottom: 10px; margin-top: 50px; }
            h3 { font-size: 1.5em; }
            h4 { font-size: 1.2em; }
            p { font-size: 1em; }
            .container { padding: 25px 0; }
            header { padding: 15px 0; }
            header .container-header { flex-direction: row; justify-content: space-between; }
            header .logo { font-size: 1.1em; margin-bottom: 0; }
            nav ul { flex-direction: row; width: auto; }
            nav ul li { margin: 0 0 0 15px; width: auto; }
            nav ul li a { font-size: 0.9em; padding: 8px 12px; }

            section { padding: 50px 20px; margin-bottom: 30px; border-radius: 12px; }
            #boas-vindas .lead { font-size: 1.15em; max-width: 750px; margin: 0 auto 25px auto; }
            #boas-vindas .campus-info { font-size: 1.3em;}

            .info-grid { grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px; }
            .info-card { padding: 25px; }
            .info-card:hover { transform: translateY(-5px) scale(1.02); box-shadow: 0 0 15px rgba(var(--rgb-destaque-neon-ciano), 0.3); }

            .disciplinas-grid { grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px; margin-top: 25px; }
            .disciplina-card { padding: 20px; }
            .disciplina-card:hover { transform: translateY(-10px) scale(1.03); box-shadow: 0 0 25px rgba(var(--rgb-destaque-neon-ciano), 0.4), 0 10px 20px rgba(0,0,0,0.4); }
            .disciplina-card-content { padding: 15px; height: calc(100% - 30px); }
            .disciplina-card .professor { font-size: 0.9em; }
            .disciplina-card .ementa-placeholder { font-size: 0.9em; }
            .disciplina-card .tag { padding: 5px 10px; font-size: 0.75em; margin-top: 15px; }

            .info-horario-geral { font-size: 1.1em; padding: 10px; margin-bottom: 25px; }
            .horario-semanal table { font-size: 0.9em; margin-top: 20px; }
            .horario-semanal th, .horario-semanal td { padding: 15px; }
            .nota-ead { margin-top: 15px; font-size: 0.9em; }

            #dicas ul li { padding: 12px 18px; font-size: 1em; }
            footer { font-size: 0.85em; padding: 30px 0; margin-top: 40px; }
        }

        @media (min-width: 992px) {
             nav ul li { margin-left: 20px; }
        }

    </style>
</head>
<body>
    <header>
        <div class="container-header">
            <div class="logo">GUIA SI <span>IFAL ARAPIRACA</span></div>
            <nav>
                <ul>
                    <li><a href="#boas-vindas">START</a></li>
                    <li><a href="#primeiro-periodo">1º PERÍODO</a></li>
                    <li><a href="#dicas">DICAS PRO</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <section id="boas-vindas">
            <h1>AVISO AOS NAVEGANTES!</h1>
            <p class="campus-info">IFAL Campus Arapiraca - Sistemas de Informação (Noturno)</p>
            <p class="lead">E aí, futuro(a) mestre dos códigos! 🚀 Bem-vindo(a) à sua nova fase no <strong>IFAL Campus Arapiraca</strong>! Preparamos este mapa estelar para você não se perder na galáxia do conhecimento do curso de <strong>Sistemas de Informação (Noturno)</strong>. Let's code!</p>
        </section>

        <section id="sobre">
            <h2>MISSÃO: SISTEMAS DE INFORMAÇÃO</h2>
            <div class="info-grid">
                <div class="info-card">
                    <h3>O que é SI? (Spoiler: É DEMAIS!)</h3>
                    <p>Sistemas de Informação é a arte e a ciência de criar soluções tecnológicas que fazem o mundo girar! Você vai aprender a construir softwares, gerenciar dados, proteger informações e muito mais. Prepare-se para ser um(a) agente de transformação digital.</p>
                </div>
                <div class="info-card">
                    <h3>IFAL ARAPIRACA: SUA BASE ESTELAR</h3>
                    <p>O <strong>IFAL Campus Arapiraca</strong> é seu novo quartel-general! Aqui você encontra laboratórios equipados, uma biblioteca cheia de segredos (e livros!), e uma galera pronta para te ajudar a decolar. Explore cada canto!</p>
                </div>
            </div>
        </section>

        <section id="primeiro-periodo">
            <h2>LEVEL 1: O INÍCIO DA JORNADA</h2>
            <h3>Suas primeiras Quests (Disciplinas):</h3>
            <div class="disciplinas-grid">
                <div class="disciplina-card">
                    <div class="disciplina-card-content">
                        <h4>ALGORITMOS E LÓGICA DE PROGRAMAÇÃO</h4>
                        <p class="professor">Instrutor: <strong>Prof. Maurício</strong></p>
                        <p class="ementa-placeholder">Desvende os segredos da lógica e dê seus primeiros passos para se tornar um(a) Jedi da programação.</p>
                    </div>
                </div>
                <div class="disciplina-card">
                    <div class="disciplina-card-content">
                        <h4>FILOSOFIA</h4>
                        <p class="professor">Instrutor: <strong>Prof. Vagner Ramalho</strong></p>
                        <p class="ementa-placeholder">"Ser ou não ser um dev?" Questione tudo e expanda sua mente para além dos códigos.</p>
                    </div>
                </div>
                <div class="disciplina-card">
                    <div class="disciplina-card-content">
                        <h4>FUNDAMENTOS DE SISTEMAS DE INFORMAÇÃO</h4>
                        <p class="professor">Instrutor: <strong>Prof. Edvonaldo</strong></p>
                        <p class="ementa-placeholder">Entenda o mapa da mina! O que são SI, para que servem e onde você se encaixa nesse universo.</p>
                    </div>
                </div>
                <div class="disciplina-card">
                    <div class="disciplina-card-content">
                        <h4>INGLÊS TÉCNICO</h4>
                        <p class="professor">Instrutor: <strong>Prof. Jean</strong></p>
                        <p class="ementa-placeholder">"The book is on the table?" Que nada! Aprenda o inglês que vai te fazer entender a documentação dos deuses da TI.</p>
                    </div>
                </div>
                <div class="disciplina-card">
                    <div class="disciplina-card-content">
                        <h4>INTRODUÇÃO ÀS TECNOLOGIAS WEB</h4>
                        <p class="professor">Instrutor: <strong>Prof. Maurício</strong></p>
                        <p class="ementa-placeholder">HTML, CSS... os blocos de construção da internet! Prepare-se para criar suas primeiras páginas. Missão via <strong>Google Classroom</strong>.</p>
                        <div>
                            <span class="tag ead">EAD</span>
                            <span class="tag classroom">Google Classroom</span>
                        </div>
                    </div>
                </div>
                <div class="disciplina-card">
                    <div class="disciplina-card-content">
                        <h4>LÓGICA MATEMÁTICA E MATEMÁTICA DISCRETA</h4>
                        <p class="professor">Instrutor: <strong>Prof. Gabriel</strong></p>
                        <p class="ementa-placeholder">A matemática por trás dos panos! Essencial para entender como a mágica da computação realmente acontece.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="horario">
            <h2>CRONOGRAMA DA MISSÃO (AULAS)</h2>
            <p class="info-horario-geral">
                Modo Noturno Ativado! Suas aulas acontecem de <strong>Segunda a Sexta, das 19h00 às 22h00</strong>.
            </p>
            <div class="horario-semanal">
                <table>
                    <thead>
                        <tr>
                            <th>Dia da Semana</th>
                            <th>Matéria em Foco</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>Segunda-feira</td>
                            <td><strong>INGLÊS TÉCNICO</strong> (Prof. Jean)</td>
                        </tr>
                        <tr>
                            <td>Terça-feira</td>
                            <td><strong>FUNDAMENTOS DE SISTEMAS DE INFORMAÇÃO</strong> (Prof. Edvonaldo)</td>
                        </tr>
                        <tr>
                            <td>Quarta-feira</td>
                            <td><strong>LÓGICA MATEMÁTICA E MATEMÁTICA DISCRETA</strong> (Prof. Gabriel)</td>
                        </tr>
                        <tr>
                            <td>Quinta-feira</td>
                            <td><strong>FILOSOFIA</strong> (Prof. Vagner Ramalho)</td>
                        </tr>
                        <tr>
                            <td>Sexta-feira</td>
                            <td><strong>ALGORITMOS E LÓGICA DE PROGRAMAÇÃO</strong> (Prof. Maurício)</td>
                        </tr>
                    </tbody>
                </table>
                <p class="nota-ead">
                    <strong>Side Quest EAD:</strong> "INTRODUÇÃO ÀS TECNOLOGIAS WEB" é sua missão online! Fique de olho no <strong>Google Classroom</strong> para atividades e cronogramas.
                </p>
            </div>
        </section>

        <section id="dicas">
            <h2>CHEAT CODES (DICAS PRO)</h2>
            <ul>
                <li><strong>Salve seu progresso:</strong> Organize-se! Use agendas, apps, o que for. Não deixe as quests acumularem.</li>
                <li><strong>Multiplayer é mais legal:</strong> Forme grupos de estudo. Trocar ideias é o melhor XP boost!</li>
                <li><strong>Explore o mapa:</strong> Conheça o IFAL Campus Arapiraca, participe de eventos, faça contatos (networking!).</li>
                <li><strong>Fale com os NPCs Sábios:</strong> Professores e veteranos são fontes de sabedoria. Pergunte, peça ajuda!</li>
                <li><strong>Não pule os tutoriais (aulas):</strong> Participe, tire dúvidas. Cada aula é uma nova skill desbloqueada.</li>
                <li><strong>Gerencie sua barra de energia:</strong> Durma bem, coma direito. Saúde em dia = mais XP no fim do dia!</li>
            </ul>
        </section>
    </main>

    <footer>
        <div class="container">
            <p class="ifal-logo-footer">IFAL ARAPIRACA - SI EDITION</p>
            <p>&copy; <script>document.write(new Date().getFullYear())</script> Guia do Calouro Intergaláctico.</p>
            <p>Boa sorte na sua jornada, Padawan!</p>
        </div>
    </footer>
    
    </body>
</html>
