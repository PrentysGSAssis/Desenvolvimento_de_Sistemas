<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Repositório de Aulas — Técnico em Desenvolvimento de Sistemas</title>
  <meta name="description" content="Aulas, conteúdos e organização de pastas para a turma de Técnico em Desenvolvimento de Sistemas." />
  <style>
    :root {
      --bg: #ffffff;
      --fg: #0f172a;     /* slate-900 */
      --muted: #e2e8f0;  /* slate-200 */
      --subtle: #64748b; /* slate-500 */
      --accent: #2563eb; /* blue-600 */
      --card: #ffffff;
      --code: #0b1220;
    }
    @media (prefers-color-scheme: dark) {
      :root {
        --bg: #0b1220;
        --fg: #e5e7eb;     /* slate-200 */
        --muted: #1f2937;  /* slate-800 */
        --subtle: #94a3b8; /* slate-400 */
        --accent: #60a5fa; /* blue-400 */
        --card: #0f172a;
        --code: #e5e7eb;
      }
    }
    /* Base */
    html, body {
      background: var(--bg);
      color: var(--fg);
      margin: 0;
      font: 16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji", sans-serif;
      -webkit-font-smoothing: antialiased;
      text-rendering: optimizeLegibility;
    }
    a { color: var(--accent); text-decoration: none; }
    a:hover, a:focus { text-decoration: underline; }
    .container { max-width: 980px; margin: 0 auto; padding: 24px; }
    header { padding: 32px 0 12px; border-bottom: 1px solid var(--muted); margin-bottom: 16px; }
    header h1 { margin: 0 0 6px; font-size: 1.75rem; }
    header p { margin: 0; color: var(--subtle); }
    nav { margin: 16px 0 8px; }
    .nav {
      display: flex; flex-wrap: wrap; gap: 8px 12px; padding: 8px 0;
    }
    .pill {
      display: inline-block; padding: 6px 10px; border: 1px solid var(--muted);
      border-radius: 999px; color: var(--fg); background: transparent;
    }
    .pill:hover { background: var(--muted); text-decoration: none; }
    section { padding: 20px 0; border-top: 1px solid var(--muted); }
    section h2 { margin: 0 0 8px; font-size: 1.25rem; }
    section p { margin: 0 0 10px; }
    /* Cards de módulos/aulas */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
      gap: 12px;
      margin-top: 8px;
    }
    .card {
      background: var(--card);
      border: 1px solid var(--muted);
      border-radius: 10px;
      padding: 14px;
      transition: transform .08s ease, box-shadow .08s ease, border-color .08s ease;
    }
    .card:hover {
      transform: translateY(-1px);
      border-color: var(--accent);
      box-shadow: 0 2px 10px rgba(0,0,0,.06);
    }
    .card h3 { margin: 0 0 6px; font-size: 1.05rem; }
    .meta { color: var(--subtle); font-size: .9rem; margin-bottom: 6px; }
    ul { margin: 8px 0 0 18px; }
    code, pre {
      font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
      background: transparent;
      color: var(--code);
    }
    pre {
      border: 1px solid var(--muted);
      border-radius: 8px;
      padding: 12px;
      overflow: auto;
      margin: 8px 0;
    }
    footer {
      margin-top: 24px;
      padding-top: 16px;
      border-top: 1px solid var(--muted);
      color: var(--subtle);
      font-size: .95rem;
    }
    .badge {
      display: inline-block;
      background: transparent;
      border: 1px solid var(--muted);
      color: var(--subtle);
      padding: 2px 8px;
      border-radius: 999px;
      font-size: .85rem;
      margin-left: 6px;
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>Repositório de Aulas — Técnico em Desenvolvimento de Sistemas <span class="badge">Base de referência</span></h1>
      <p>Professor: <strong>[Seu Nome]</strong> • Objetivo: facilitar o acesso às aulas e conteúdos, e oferecer um modelo de organização de arquivos para os alunos espelharem.</p>
      <nav>
        <div class="nav">
          <a class="pill" href="#apresentacao">Apresentação</a>
          <a class="pill" href="#como-usar">Como usar</a>
          <a class="pill" href="#estrutura">Estrutura de pastas</a>
          <a class="pill" href="#modulos">Módulos e aulas</a>
          <a class="pill" href="#links">Links importantes</a>
          <a class="pill" href="#contato">Contato e licença</a>
        </div>
      </nav>
    </header>

    <section id="apresentacao">
      <h2>Apresentação</h2>
      <p>Este repositório foi criado por mim, professor da turma, para centralizar materiais das aulas, orientar estudos e servir como referência para a <em>organização de arquivos</em>. Os alunos são convidados a manter nos seus próprios repositórios uma estrutura similar à apresentada abaixo.</p>
    </section>

    <section id="como-usar">
      <h2>Como usar</h2>
      <ol>
        <li>Acompanhe o cronograma no bloco “Módulos e aulas” e abra o link de cada aula.</li>
        <li>Baixe ou clone este repositório e replique a estrutura de pastas no seu projeto pessoal.</li>
        <li>Para cada aula, crie sua própria pasta espelhando o modelo e salve códigos, anotações e exercícios.</li>
        <li>Use os “Links importantes” para acessar slides, gravações e comunicados.</li>
      </ol>
    </section>

    <section id="estrutura">
      <h2>Estrutura de pastas recomendada</h2>
      <pre><code>/
├─ 01-introducao/
│  ├─ README.md
│  ├─ exercicios/
│  └─ exemplos/
├─ 02-logica-programacao/
│  ├─ README.md
│  ├─ exercicios/
│  └─ exemplos/
├─ 03-poo/
│  ├─ README.md
│  ├─ exercicios/
│  └─ exemplos/
├─ assets/
│  ├─ slides/
│  └─ datasets/
└─ docs/   ← materiais gerais e anotações</code></pre>
      <p>Adapte os nomes conforme a ementa da sua turma. Cada pasta de módulo deve conter um <code>README.md</code> com objetivos, conteúdo e tarefas.</p>
    </section>

    <section id="modulos">
      <h2>Módulos e aulas</h2>
      <div class="grid">
        <article class="card">
          <h3>01 — Introdução ao curso</h3>
          <div class="meta">Semana 1 • Fundamentos • Ambiente</div>
          <ul>
            <li><a href="[LINK-DA-AULA-1]">Aula 1: Apresentação do curso e ferramentas</a></li>
            <li><a href="[LINK-DA-AULA-2]">Aula 2: Git e GitHub — fluxo básico</a></li>
          </ul>
        </article>
        <article class="card">
          <h3>02 — Lógica de Programação</h3>
          <div class="meta">Semanas 2–4 • Variáveis • Condições • Laços</div>
          <ul>
            <li><a href="[LINK-DA-AULA-3]">Aula 3: Tipos e operadores</a></li>
            <li><a href="[LINK-DA-AULA-4]">Aula 4: Estruturas de decisão</a></li>
            <li><a href="[LINK-DA-AULA-5]">Aula 5: Laços de repetição</a></li>
          </ul>
        </article>
        <article class="card">
          <h3>03 — POO</h3>
          <div class="meta">Semanas 5–7 • Classes • Objetos • Encapsulamento</div>
          <ul>
            <li><a href="[LINK-DA-AULA-6]">Aula 6: Conceitos de POO</a></li>
            <li><a href="[LINK-DA-AULA-7]">Aula 7: Herança e Polimorfismo</a></li>
          </ul>
        </article>
        <article class="card">
          <h3>04 — Web e APIs</h3>
          <div class="meta">Semanas 8–10 • HTTP • REST • JSON</div>
          <ul>
            <li><a href="[LINK-DA-AULA-8]">Aula 8: HTTP e REST</a></li>
            <li><a href="[LINK-DA-AULA-9]">Aula 9: Consumo de APIs</a></li>
          </ul>
        </article>
        <!--
          Dica: duplique os cards acima e ajuste títulos/links conforme o seu plano.
          Exclua este comentário no seu arquivo final.
        -->
      </div>
    </section>

    <section id="links">
      <h2>Links importantes</h2>
      <ul>
        <li><a href="[LINK-DA-ORGANIZACAO-GH]">Organização no GitHub da turma</a></li>
        <li><a href="[LINK-DOS-SLIDES]">Slides e materiais</a></li>
        <li><a href="[LINK-DA-PLATAFORMA]">Plataforma de aula/gravações</a></li>
        <li><a href="[LINK-DO-CALENDARIO]">Calendário da disciplina</a></li>
      </ul>
    </section>

    <section id="contato">
      <h2>Contato e licença</h2>
      <p>Para dúvidas, use os canais oficiais da turma ou abra uma <a href="[LINK-ISSUES]">issue</a> neste repositório. Sugestões e correções são bem-vindas via pull request.</p>
      <p>Licença: <a href="[LINK-DA-LICENCA]">[Tipo de licença]</a>. Se reutilizar, mantenha créditos e referências.</p>
    </section>

    <footer>
      <p>Atualize os campos entre colchetes com seus links. Para uma boa experiência, ative o GitHub Pages e aponte para este index.html.</p>
    </footer>
  </div>
</body>
</html>
