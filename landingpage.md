# Atividade: Landing Page do Curso de Análise e Desenvolvimento de Sistemas

## 📋 Objetivo da Atividade

Criar uma landing page profissional em HTML5 e CSS3 para apresentar o curso de Tecnologia em Análise e Desenvolvimento de Sistemas do IFRN. A página deve ser informativa, atrativa e responsiva, seguindo as melhores práticas de desenvolvimento web.

## 🎯 Seções Obrigatórias da Landing Page

A landing page deve conter **pelo menos** as seguintes seções:

### 1. **Informações Gerais**

- Nome completo do curso
- Nome do coordenador do curso
- Logo ou banner do curso/instituição

### 2. **Perfil do Curso**

- Apresentação do curso
- Objetivos do curso
- Diferenciais e destaques

### 3. **Perfil de Atuação do Profissional**

- Áreas de atuação
- Competências desenvolvidas
- Mercado de trabalho

### 4. **Ficha Técnica**

- Duração do curso
- Carga horária total
- Turno(s) de oferta
- Modalidade de ensino
- Tipo de certificação

---

## 📚 Onde Coletar as Informações

Para realizar esta atividade, você deve consultar a **página oficial do curso**:

🔗 **Link oficial:** [Página do curso TADS - IFRN](https://diatinf.ifrn.edu.br/cursos/tecnologia-em-analise-e-desenvolvimento-de-sistemas/)

**Importante:** Utilize informações oficiais e atualizadas do site. Certifique-se de ler com atenção todas as seções disponíveis na página oficial para extrair o conteúdo necessário.

---

## 💻 Estrutura Sugerida da Landing Page

### Exemplo de Estrutura HTML `landingpage.html`

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tecnologia em Análise e Desenvolvimento de Sistemas - IFRN</title>
    <link rel="stylesheet" href="landingpage.css">
</head>
<body>
    <!-- Header/Navegação -->
    <header>
        <nav>
            <div class="container">
                <h1>IFRN - Campus Natal Central</h1>
                <ul class="nav-menu">
                    <li><a href="#informacoes">Informações</a></li>
                    <li><a href="#perfil-curso">Perfil do Curso</a></li>
                    <li><a href="#atuacao">Atuação Profissional</a></li>
                    <li><a href="#ficha-tecnica">Ficha Técnica</a></li>
                </ul>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1>Tecnologia em Análise e Desenvolvimento de Sistemas</h1>
            <p class="hero-subtitle">Transforme o futuro através da tecnologia</p>
            <a href="#informacoes" class="btn-cta">Conheça o Curso</a>
        </div>
    </section>

    <!-- Seção 1: Informações Gerais -->
    <section id="informacoes" class="section">
        <div class="container">
            <h2>Informações Gerais</h2>
            <div class="info-box">
                <h3>Nome do Curso</h3>
                <p>Curso Superior de Tecnologia em Análise e Desenvolvimento de Sistemas</p>
            </div>
            <div class="info-box">
                <h3>Coordenação</h3>
                <p><strong>Coordenador(a):</strong> [Nome do Coordenador - consulte o site oficial]</p>
            </div>
            <div class="info-box">
                <h3>Instituição</h3>
                <p>Instituto Federal de Educação, Ciência e Tecnologia do Rio Grande do Norte (IFRN)</p>
                <p>Campus Natal - Central</p>
            </div>
        </div>
    </section>

    <!-- Seção 2: Perfil do Curso -->
    <section id="perfil-curso" class="section bg-light">
        <div class="container">
            <h2>Perfil do Curso</h2>
            <div class="content-grid">
                <div class="content-card">
                    <h3>Sobre o Curso</h3>
                    <p>[Adicione aqui a apresentação do curso disponível no site oficial]</p>
                </div>
                <div class="content-card">
                    <h3>Objetivos</h3>
                    <p>[Adicione aqui os objetivos do curso disponíveis no site oficial]</p>
                </div>
                <div class="content-card">
                    <h3>Diferenciais</h3>
                    <ul>
                        <li>Corpo docente qualificado</li>
                        <li>Infraestrutura moderna</li>
                        <li>Projetos práticos</li>
                        <li>Parcerias com empresas</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção 3: Perfil de Atuação Profissional -->
    <section id="atuacao" class="section">
        <div class="container">
            <h2>Perfil de Atuação do Profissional</h2>
            <div class="atuacao-grid">
                <div class="atuacao-card">
                    <h3>Áreas de Atuação</h3>
                    <ul>
                        <li>Desenvolvimento de software</li>
                        <li>Análise de sistemas</li>
                        <li>Gerenciamento de projetos</li>
                        <li>Consultoria em TI</li>
                        <li>Banco de dados</li>
                    </ul>
                </div>
                <div class="atuacao-card">
                    <h3>Competências Desenvolvidas</h3>
                    <ul>
                        <li>Programação em múltiplas linguagens</li>
                        <li>Desenvolvimento web e mobile</li>
                        <li>Modelagem de sistemas</li>
                        <li>Gestão de banco de dados</li>
                        <li>Metodologias ágeis</li>
                    </ul>
                </div>
                <div class="atuacao-card">
                    <h3>Mercado de Trabalho</h3>
                    <p>[Adicione informações sobre o mercado de trabalho disponíveis no site oficial]</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Seção 4: Ficha Técnica -->
    <section id="ficha-tecnica" class="section bg-light">
        <div class="container">
            <h2>Ficha Técnica do Curso</h2>
            <table class="ficha-table">
                <tbody>
                    <tr>
                        <th>Duração</th>
                        <td>[Consulte o site oficial]</td>
                    </tr>
                    <tr>
                        <th>Carga Horária Total</th>
                        <td>[Consulte o site oficial]</td>
                    </tr>
                    <tr>
                        <th>Turno</th>
                        <td>[Consulte o site oficial]</td>
                    </tr>
                    <tr>
                        <th>Modalidade</th>
                        <td>Presencial</td>
                    </tr>
                    <tr>
                        <th>Certificação</th>
                        <td>Tecnólogo em Análise e Desenvolvimento de Sistemas</td>
                    </tr>
                    <tr>
                        <th>Forma de Ingresso</th>
                        <td>[Consulte o site oficial]</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>© 2025 IFRN - Instituto Federal do Rio Grande do Norte</p>
            <p>Campus Natal - Central</p>
            <div class="footer-links">
                <a href="https://diatinf.ifrn.edu.br/cursos/tecnologia-em-analise-e-desenvolvimento-de-sistemas/" target="_blank">Site Oficial do Curso</a>
                <a href="https://portal.ifrn.edu.br/" target="_blank">Portal IFRN</a>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Exemplo de Estilização CSS `landingpage.css`

```css
/* Reset e configurações básicas */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* CSS Custom Properties (Variáveis) */
:root {
    --primary-color: #1a472a;
    --secondary-color: #ff6b35;
    --light-bg: #f8f9fa;
    --text-color: #333;
    --text-secondary: #555;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    line-height: 1.6;
    color: var(--text-color);
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header e Navegação */
header {
    background-color: var(--primary-color);
    color: white;
    padding: 1rem 0;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

header h1 {
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
}

.nav-menu {
    list-style: none;
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
}

.nav-menu li a {
    color: white;
    text-decoration: none;
    padding: 5px 10px;
    border-radius: 5px;
    transition: background-color 0.3s;
}

.nav-menu li a:hover {
    background-color: rgba(255, 255, 255, 0.2);
}

/* Hero Section */
.hero {
    background: linear-gradient(135deg, var(--primary-color) 0%, #2d7a4d 100%);
    color: white;
    padding: 150px 20px 100px;
    text-align: center;
    margin-top: 80px;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.hero-subtitle {
    font-size: 1.5rem;
    margin-bottom: 2rem;
    opacity: 0.9;
}

.btn-cta {
    display: inline-block;
    background-color: var(--secondary-color);
    color: white;
    padding: 15px 40px;
    text-decoration: none;
    border-radius: 50px;
    font-size: 1.2rem;
    font-weight: bold;
    transition: transform 0.3s, box-shadow 0.3s;
}

.btn-cta:hover {
    transform: translateY(-3px);
    box-shadow: 0 5px 15px rgba(255, 107, 53, 0.4);
}

/* Seções */
.section {
    padding: 80px 20px;
}

.bg-light {
    background-color: var(--light-bg);
}

.section h2 {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 3rem;
    color: var(--primary-color);
    position: relative;
}

.section h2::after {
    content: '';
    display: block;
    width: 80px;
    height: 4px;
    background-color: var(--secondary-color);
    margin: 20px auto 0;
    border-radius: 2px;
}

/* Info Boxes */
.info-box {
    background-color: white;
    padding: 30px;
    margin-bottom: 20px;
    border-radius: 10px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    transition: transform 0.3s;
}

.info-box:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 20px rgba(0,0,0,0.15);
}

.info-box h3 {
    color: var(--primary-color);
    margin-bottom: 15px;
    font-size: 1.5rem;
}

/* Content Grid */
.content-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
    margin-top: 40px;
}

.content-card {
    background-color: white;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
}

.content-card h3 {
    color: var(--primary-color);
    margin-bottom: 15px;
    font-size: 1.3rem;
}

.content-card ul {
    list-style-position: inside;
    color: var(--text-secondary);
}

.content-card ul li {
    padding: 8px 0;
    border-bottom: 1px solid #eee;
}

.content-card ul li:last-child {
    border-bottom: none;
}

/* Atuação Grid */
.atuacao-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 30px;
}

.atuacao-card {
    background-color: white;
    padding: 30px;
    border-radius: 10px;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
    border-left: 5px solid var(--primary-color);
}

.atuacao-card h3 {
    color: var(--primary-color);
    margin-bottom: 20px;
    font-size: 1.4rem;
}

.atuacao-card ul {
    list-style: none;
}

.atuacao-card ul li {
    padding: 10px 0;
    padding-left: 25px;
    position: relative;
}

.atuacao-card ul li::before {
    content: '✓';
    position: absolute;
    left: 0;
    color: var(--secondary-color);
    font-weight: bold;
}

/* Ficha Técnica Table */
.ficha-table {
    width: 100%;
    max-width: 800px;
    margin: 0 auto;
    background-color: white;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 3px 10px rgba(0,0,0,0.1);
}

.ficha-table th,
.ficha-table td {
    padding: 20px;
    text-align: left;
    border-bottom: 1px solid #eee;
}

.ficha-table th {
    background-color: var(--primary-color);
    color: white;
    font-weight: bold;
    width: 40%;
}

.ficha-table td {
    color: var(--text-secondary);
}

.ficha-table tr:last-child th,
.ficha-table tr:last-child td {
    border-bottom: none;
}

/* Footer */
footer {
    background-color: var(--primary-color);
    color: white;
    padding: 40px 20px;
    text-align: center;
}

footer p {
    margin-bottom: 10px;
}

.footer-links {
    margin-top: 20px;
}

.footer-links a {
    color: white;
    text-decoration: none;
    margin: 0 15px;
    padding: 8px 15px;
    border: 1px solid white;
    border-radius: 5px;
    transition: background-color 0.3s;
}

.footer-links a:hover {
    background-color: rgba(255, 255, 255, 0.2);
}

/* Responsividade */
@media (max-width: 768px) {
    .hero-content h1 {
        font-size: 2rem;
    }
  
    .hero-subtitle {
        font-size: 1.2rem;
    }
  
    .section h2 {
        font-size: 2rem;
    }
  
    .nav-menu {
        flex-direction: column;
    }
  
    .content-grid,
    .atuacao-grid {
        grid-template-columns: 1fr;
    }
  
    .ficha-table th,
    .ficha-table td {
        display: block;
        width: 100%;
    }
  
    .ficha-table th {
        border-bottom: none;
        padding-bottom: 10px;
    }
}
```

---

## ✅ Checklist da Atividade

### Preparação

- [X] Acessar o site oficial do curso: https://diatinf.ifrn.edu.br/cursos/tecnologia-em-analise-e-desenvolvimento-de-sistemas/
- [X] Ler todas as informações disponíveis no site
- [X] Anotar os dados necessários para cada seção

### Estrutura HTML

- [X] Criar arquivo `landingpage.html` com estrutura HTML5 válida
- [X] Definir `<meta charset="UTF-8">` e viewport para responsividade
- [X] Criar título descritivo na tag `<title>`
- [X] Adicionar link para arquivo CSS externo

### Navegação

- [X] Implementar menu de navegação com links para as seções
- [X] Garantir que os links de navegação funcionem corretamente (navegação âncora)

### Seção 1: Informações Gerais

- [X] Adicionar nome completo do curso
- [X] Incluir nome do coordenador (consultar site oficial)
- [X] Adicionar informações sobre a instituição

### Seção 2: Perfil do Curso

- [X] Apresentar o curso com base nas informações oficiais
- [X] Listar os objetivos do curso
- [X] Destacar diferenciais e características especiais

### Seção 3: Perfil de Atuação

- [X] Listar áreas de atuação do profissional
- [X] Descrever competências desenvolvidas no curso
- [X] Incluir informações sobre mercado de trabalho

### Seção 4: Ficha Técnica

- [X] Criar tabela com informações técnicas do curso
- [X] Incluir duração do curso
- [X] Adicionar carga horária total
- [X] Especificar turno de oferta
- [X] Informar modalidade de ensino
- [X] Indicar tipo de certificação

### Estilização CSS

- [X] Criar arquivo `landingpage.css`
- [X] Aplicar reset CSS básico
- [X] Estilizar header e navegação
- [X] Criar hero section atrativa
- [X] Estilizar todas as seções com cores e espaçamentos adequados
- [X] Estilizar a tabela da ficha técnica
- [X] Criar footer com links úteis

### Responsividade

- [X] Implementar media queries para dispositivos móveis
- [X] Testar layout em diferentes tamanhos de tela
- [X] Garantir que o menu seja utilizável em mobile
- [X] Verificar legibilidade em telas pequenas

### Qualidade e Validação

- [X] Validar HTML no [W3C Validator](https://validator.w3.org/)
- [X] Validar CSS no [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- [X] Verificar se todas as informações estão corretas e atualizadas
- [X] Revisar ortografia e gramática
- [X] Testar todos os links

### Entrega

- [X] Código bem indentado e organizado
- [X] Comentários explicativos quando necessário
- [X] Commit no GitHub com mensagem descritiva
- [X] Verificar se a página está funcionando corretamente

---

## 🎨 Dicas de Design

1. **Paleta de Cores**: Use as cores institucionais do IFRN (recomenda-se definir variáveis CSS como `--primary-color: #1a472a` para facilitar a manutenção)
2. **Tipografia**: Escolha fontes legíveis e profissionais
3. **Imagens**: Se possível, adicione imagens relacionadas ao curso ou ao campus
4. **Espaçamento**: Use espaçamentos generosos para melhorar a legibilidade
5. **Hierarquia Visual**: Use tamanhos de fonte e cores para criar hierarquia clara
6. **Call-to-Action**: Destaque botões ou links importantes com cores contrastantes
7. **Variáveis CSS**: Utilize CSS custom properties (variáveis) para manter consistência e facilitar alterações futuras

---

## 🚀 Desafios Extras (Opcional)

Se você quiser ir além, experimente:

1. **Carrossel de Imagens**: Adicione um carrossel na hero section com imagens do curso
2. **Animações**: Implemente animações suaves ao rolar a página
3. **Depoimentos**: Adicione uma seção com depoimentos de alunos ou egressos
4. **FAQ**: Crie uma seção de perguntas frequentes
5. **Formulário de Contato**: Adicione um formulário para interessados
6. **Ícones**: Use Font Awesome ou similar para adicionar ícones nas seções
7. **Galeria**: Crie uma galeria de fotos do campus e laboratórios
8. **Vídeo**: Incorpore um vídeo de apresentação do curso
9. **Modo Escuro**: Implemente um toggle para modo escuro
10. **Acessibilidade**: Melhore a acessibilidade com ARIA labels e navegação por teclado

---

## 📚 Recursos Úteis

- **Site Oficial do Curso**: [TADS IFRN](https://diatinf.ifrn.edu.br/cursos/tecnologia-em-analise-e-desenvolvimento-de-sistemas/)
- **MDN Web Docs - HTML**: [https://developer.mozilla.org/pt-BR/docs/Web/HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
- **MDN Web Docs - CSS**: [https://developer.mozilla.org/pt-BR/docs/Web/CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
- **W3C HTML Validator**: [https://validator.w3.org/](https://validator.w3.org/)
- **W3C CSS Validator**: [https://jigsaw.w3.org/css-validator/](https://jigsaw.w3.org/css-validator/)
- **Google Fonts**: [https://fonts.google.com/](https://fonts.google.com/)
- **Font Awesome Icons**: [https://fontawesome.com/](https://fontawesome.com/)
- **CSS Tricks**: [https://css-tricks.com/](https://css-tricks.com/)
- **Can I Use**: [https://caniuse.com/](https://caniuse.com/) (verificar compatibilidade de recursos)

---

## 🎓 Critérios de Avaliação

| Critério                      | Peso | Descrição                                                            |
| ------------------------------ | ---- | ---------------------------------------------------------------------- |
| **Conteúdo**            | 30%  | Todas as seções obrigatórias presentes e com informações corretas |
| **Estrutura HTML**       | 20%  | Uso correto e semântico de tags HTML5                                 |
| **Estilização CSS**    | 25%  | Design atrativo, profissional e coerente                               |
| **Responsividade**       | 15%  | Layout adaptável para diferentes dispositivos                         |
| **Qualidade do Código** | 10%  | Código limpo, organizado e bem comentado                              |

---

## ❓ Perguntas Frequentes

**Q: Posso usar frameworks CSS como Bootstrap?**
A: Sim, mas recomenda-se criar o CSS do zero para praticar os conceitos aprendidos.

**Q: É obrigatório usar as cores sugeridas?**
A: Não, você pode personalizar as cores, mas mantenha um design profissional e harmonioso.

**Q: Posso adicionar mais seções além das obrigatórias?**
A: Sim! Sinta-se livre para adicionar seções extras que enriqueçam a landing page.

**Q: Como faço para validar meu HTML?**
A: Acesse https://validator.w3.org/, cole seu código ou faça upload do arquivo.

**Q: O que é uma landing page?**
A: É uma página web focada em apresentar um produto, serviço ou curso de forma objetiva e atrativa, com o objetivo de converter visitantes em interessados.

---

**Bons estudos e mãos à obra! 💻🚀**

*Esta atividade foi desenvolvida para a disciplina de Web Design do IFRN.*
