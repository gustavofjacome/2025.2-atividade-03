# Atividade: Replicando a Interface do Google Gemini

## 📋 Objetivo da Atividade

Criar uma réplica da interface do Google Gemini em HTML5 e CSS3, reproduzindo fielmente o layout, cores e elementos visuais da aplicação.

## 🎯 Descrição

Você deve replicar a interface principal do Google Gemini conforme mostrado na imagem `gemini.png` (em anexo). A interface contém três áreas principais:

### 1. **Barra Lateral Esquerda (Sidebar)**

- Ícone de menu hambúrguer
- Botão "Nova conversa" com ícone de edição e botão de expandir
- Opção "Veja alguns Gems" com ícone de diamante
- Seção "Recentes" com lista de conversas anteriores:
  - O Que é Uma Landing Page
  - Tradução de "Tie" para Português
  - Tradução de Frase Poética em Inglês
  - como avaliação introdutória de html ...
  - Box-sizing: Border-box para layouts
  - KORE11: Rendimentos 2025 em JSON
  - CSS Display: Valores e Exemplos
  - Corpo dos Fungos: Hifas e Micélio
- Link "Configurações e ajuda" no rodapé com ícone de engrenagem

### 2. **Barra Superior (Header)**

- Ícone de busca
- Logo/título "Gemini"
- Botão "Faça upgrade para o Google AI Plus" com ícone de estrela/sparkle
- Foto de perfil do usuário

### 3. **Área de Conteúdo Principal**

- Mensagem de boas-vindas centralizada: "Olá, Leonardo" (em azul)
- Campo de entrada "Peça ao Gemini" com:
  - Ícone de adicionar (+)
  - Botão "Ferramentas" com ícone
  - Seletor "2.5 Pro" com dropdown
  - Ícone de microfone para entrada por voz

---

## 💻 Código Inicial

### Arquivo `replica.html`

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gemini - Google AI</title>
    <link rel="stylesheet" href="replica.css">
</head>
<body>
    <!-- Barra Lateral -->
    <aside class="sidebar">
        <!-- Menu Hambúrguer -->
        <div class="sidebar-header">
            <button class="menu-btn" aria-label="Menu">
                <span class="menu-icon">☰</span>
            </button>
        </div>

        <!-- Nova Conversa -->
        <div class="new-chat">
            <button class="new-chat-btn">
                <span class="icon">✏️</span>
                <span class="text">Nova conversa</span>
            </button>
            <button class="expand-btn" aria-label="Expandir">
                <span class="icon">⛶</span>
            </button>
        </div>

        <!-- Veja alguns Gems -->
        <div class="gems-section">
            <button class="gems-btn">
                <span class="icon">♦️</span>
                <span class="text">Veja alguns Gems</span>
            </button>
        </div>

        <!-- Seção Recentes -->
        <div class="recent-section">
            <h3>Recentes</h3>
            <ul class="recent-list">
                <li><a href="#">O Que é Uma Landing Page</a></li>
                <li><a href="#">Tradução de "Tie" para Português</a></li>
                <li><a href="#">Tradução de Frase Poética em Inglês</a></li>
                <li><a href="#">como avaliação introdutória de html ...</a></li>
                <li><a href="#">Box-sizing: Border-box para layouts</a></li>
                <li><a href="#">KORE11: Rendimentos 2025 em JSON</a></li>
                <li><a href="#">CSS Display: Valores e Exemplos</a></li>
                <li><a href="#">Corpo dos Fungos: Hifas e Micélio</a></li>
            </ul>
        </div>

        <!-- Configurações -->
        <div class="sidebar-footer">
            <button class="settings-btn">
                <span class="icon">⚙️</span>
                <span class="text">Configurações e ajuda</span>
            </button>
        </div>
    </aside>

    <!-- Conteúdo Principal -->
    <main class="main-content">
        <!-- Barra Superior -->
        <header class="top-bar">
            <div class="top-bar-left">
                <button class="search-btn" aria-label="Buscar">
                    <span class="icon">🔍</span>
                </button>
                <h1 class="logo">Gemini</h1>
            </div>
            <div class="top-bar-right">
                <button class="upgrade-btn">
                    <span class="icon">✨</span>
                    <span class="text">Faça upgrade para o Google AI Plus</span>
                </button>
                <div class="profile-pic">
                    <img src="https://via.placeholder.com/40" alt="Perfil do usuário">
                </div>
            </div>
        </header>

        <!-- Área de Chat -->
        <div class="chat-area">
            <div class="welcome-message">
                <h2>Olá, Leonardo</h2>
            </div>

            <!-- Campo de Entrada -->
            <div class="input-container">
                <div class="input-box">
                    <input type="text" placeholder="Peça ao Gemini" class="chat-input">
                    <div class="input-actions">
                        <button class="action-btn" aria-label="Adicionar">
                            <span class="icon">+</span>
                        </button>
                        <button class="tools-btn">
                            <span class="icon">🛠️</span>
                            <span class="text">Ferramentas</span>
                        </button>
                        <button class="version-selector">
                            <span class="text">2.5 Pro</span>
                            <span class="icon">▼</span>
                        </button>
                        <button class="mic-btn" aria-label="Microfone">
                            <span class="icon">🎤</span>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </main>
</body>
</html>
```

### Arquivo `replica.css`

```css
/* Reset e Configurações Globais */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Variáveis CSS */
:root {
    --sidebar-bg: #f8f9fa;
    --sidebar-width: 280px;
    --primary-color: #1a73e8;
    --text-primary: #202124;
    --text-secondary: #5f6368;
    --hover-bg: #e8eaed;
    --border-color: #dadce0;
    --input-bg: #f1f3f4;
    --white: #ffffff;
}

body {
    font-family: 'Google Sans', 'Roboto', Arial, sans-serif;
    color: var(--text-primary);
    height: 100vh;
    display: flex;
    overflow: hidden;
}

/* Barra Lateral */
.sidebar {
    width: var(--sidebar-width);
    background-color: var(--sidebar-bg);
    display: flex;
    flex-direction: column;
    padding: 8px;
    border-right: 1px solid var(--border-color);
    overflow-y: auto;
}

.sidebar-header {
    padding: 8px;
    margin-bottom: 8px;
}

.menu-btn {
    background: none;
    border: none;
    cursor: pointer;
    padding: 8px;
    border-radius: 50%;
    font-size: 20px;
    color: var(--text-secondary);
    transition: background-color 0.2s;
}

.menu-btn:hover {
    background-color: var(--hover-bg);
}

/* Nova Conversa */
.new-chat {
    display: flex;
    gap: 4px;
    margin-bottom: 16px;
}

.new-chat-btn {
    flex: 1;
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 12px 16px;
    background: var(--white);
    border: 1px solid var(--border-color);
    border-radius: 24px;
    cursor: pointer;
    font-size: 14px;
    color: var(--text-secondary);
    transition: all 0.2s;
}

.new-chat-btn:hover {
    background-color: var(--hover-bg);
    box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}

.expand-btn {
    padding: 12px;
    background: var(--white);
    border: 1px solid var(--border-color);
    border-radius: 50%;
    cursor: pointer;
    font-size: 14px;
    color: var(--text-secondary);
    transition: background-color 0.2s;
}

.expand-btn:hover {
    background-color: var(--hover-bg);
}

/* Veja alguns Gems */
.gems-section {
    margin-bottom: 16px;
}

.gems-btn {
    width: 100%;
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 10px 16px;
    background: none;
    border: none;
    border-radius: 24px;
    cursor: pointer;
    font-size: 14px;
    color: var(--text-secondary);
    transition: background-color 0.2s;
}

.gems-btn:hover {
    background-color: var(--hover-bg);
}

/* Seção Recentes */
.recent-section {
    flex: 1;
    overflow-y: auto;
}

.recent-section h3 {
    font-size: 11px;
    font-weight: 500;
    color: var(--text-secondary);
    text-transform: uppercase;
    letter-spacing: 0.8px;
    padding: 12px 16px 8px;
}

.recent-list {
    list-style: none;
}

.recent-list li {
    margin-bottom: 2px;
}

.recent-list a {
    display: block;
    padding: 10px 16px;
    color: var(--text-primary);
    text-decoration: none;
    font-size: 14px;
    border-radius: 24px;
    transition: background-color 0.2s;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
}

.recent-list a:hover {
    background-color: var(--hover-bg);
}

/* Rodapé da Sidebar */
.sidebar-footer {
    margin-top: auto;
    padding-top: 16px;
}

.settings-btn {
    width: 100%;
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 10px 16px;
    background: none;
    border: none;
    border-radius: 24px;
    cursor: pointer;
    font-size: 14px;
    color: var(--text-secondary);
    transition: background-color 0.2s;
}

.settings-btn:hover {
    background-color: var(--hover-bg);
}

/* Conteúdo Principal */
.main-content {
    flex: 1;
    display: flex;
    flex-direction: column;
    background-color: var(--white);
    overflow: hidden;
}

/* Barra Superior */
.top-bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 12px 24px;
    border-bottom: 1px solid var(--border-color);
}

.top-bar-left,
.top-bar-right {
    display: flex;
    align-items: center;
    gap: 16px;
}

.search-btn {
    background: none;
    border: none;
    cursor: pointer;
    padding: 8px;
    border-radius: 50%;
    font-size: 20px;
    color: var(--text-secondary);
    transition: background-color 0.2s;
}

.search-btn:hover {
    background-color: var(--hover-bg);
}

.logo {
    font-size: 22px;
    font-weight: 400;
    color: var(--text-secondary);
}

.upgrade-btn {
    display: flex;
    align-items: center;
    gap: 8px;
    padding: 8px 16px;
    background: var(--white);
    border: 1px solid var(--border-color);
    border-radius: 20px;
    cursor: pointer;
    font-size: 14px;
    color: var(--text-primary);
    transition: all 0.2s;
}

.upgrade-btn:hover {
    background-color: var(--hover-bg);
    box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1);
}

.profile-pic {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    overflow: hidden;
}

.profile-pic img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* Área de Chat */
.chat-area {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 32px;
    overflow-y: auto;
}

.welcome-message {
    margin-bottom: 48px;
}

.welcome-message h2 {
    font-size: 48px;
    font-weight: 400;
    color: var(--primary-color);
    text-align: center;
}

/* Campo de Entrada */
.input-container {
    width: 100%;
    max-width: 880px;
}

.input-box {
    background-color: var(--input-bg);
    border-radius: 32px;
    padding: 16px 24px;
    display: flex;
    flex-direction: column;
    gap: 12px;
    box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
}

.chat-input {
    background: none;
    border: none;
    outline: none;
    font-size: 16px;
    color: var(--text-primary);
    width: 100%;
}

.chat-input::placeholder {
    color: var(--text-secondary);
}

.input-actions {
    display: flex;
    align-items: center;
    gap: 8px;
}

.action-btn,
.tools-btn,
.version-selector,
.mic-btn {
    background: none;
    border: none;
    cursor: pointer;
    padding: 8px 12px;
    border-radius: 16px;
    font-size: 14px;
    color: var(--text-secondary);
    display: flex;
    align-items: center;
    gap: 6px;
    transition: background-color 0.2s;
}

.action-btn:hover,
.tools-btn:hover,
.version-selector:hover,
.mic-btn:hover {
    background-color: var(--hover-bg);
}

.version-selector {
    margin-left: auto;
}

/* Responsividade */
@media (max-width: 768px) {
    .sidebar {
        position: fixed;
        left: -280px;
        top: 0;
        bottom: 0;
        z-index: 1000;
        transition: left 0.3s;
    }

    .sidebar.open {
        left: 0;
    }

    .top-bar {
        padding: 12px 16px;
    }

    .upgrade-btn .text {
        display: none;
    }

    .welcome-message h2 {
        font-size: 32px;
    }

    .input-box {
        padding: 12px 16px;
    }

    .tools-btn .text,
    .version-selector .text {
        display: none;
    }
}
```

---

## ✅ Checklist da Atividade

### Preparação

- [X] Visualizar a imagem `gemini.png` para entender o layout
- [X] Criar arquivo `replica.html`
- [X] Criar arquivo `replica.css`
- [X] Copiar o código inicial fornecido acima

### Estrutura HTML - Sidebar

- [X] Implementar o menu hambúrguer no topo da sidebar
- [X] Adicionar botão "Nova conversa" com ícone de edição
- [X] Adicionar botão de expandir ao lado de "Nova conversa"
- [X] Criar seção "Veja alguns Gems" com ícone de diamante
- [X] Implementar seção "Recentes" com título
- [X] Adicionar lista de 8 conversas recentes
- [X] Criar link "Configurações e ajuda" no rodapé com ícone de engrenagem

### Estrutura HTML - Barra Superior

- [X] Adicionar ícone de busca à esquerda
- [X] Inserir logo/título "Gemini"
- [X] Criar botão "Faça upgrade para o Google AI Plus" com ícone
- [X] Adicionar foto de perfil do usuário

### Estrutura HTML - Área Principal

- [X] Criar mensagem de boas-vindas "Olá, Leonardo"
- [X] Implementar campo de entrada "Peça ao Gemini"
- [X] Adicionar botão "+" (adicionar)
- [X] Adicionar botão "Ferramentas" com ícone
- [X] Criar seletor de versão "2.5 Pro" com dropdown
- [X] Adicionar ícone de microfone

### Estilização CSS - Layout Geral

- [X] Configurar display flex para body (sidebar + conteúdo)
- [X] Definir largura fixa para sidebar (280px)
- [X] Configurar área principal para ocupar espaço restante
- [X] Aplicar overflow adequado em cada seção

### Estilização CSS - Cores e Tipografia

- [X] Definir variáveis CSS para cores principais
- [X] Aplicar cor de fundo cinza claro na sidebar (#f8f9fa)
- [X] Configurar cor de texto primária (#202124)
- [X] Aplicar cor azul do Google (#1a73e8) na mensagem de boas-vindas
- [X] Usar fonte 'Google Sans' ou 'Roboto' como fallback

### Estilização CSS - Sidebar

- [X] Estilizar botão "Nova conversa" com borda arredondada
- [X] Aplicar hover effects nos botões da sidebar
- [X] Estilizar lista de conversas recentes
- [X] Adicionar efeito de truncamento de texto (ellipsis) nos itens longos
- [X] Posicionar "Configurações e ajuda" no final da sidebar

### Estilização CSS - Barra Superior

- [X] Alinhar elementos da barra superior (esquerda e direita)
- [X] Estilizar botão de upgrade com borda e hover effect
- [X] Fazer foto de perfil circular (border-radius: 50%)
- [X] Adicionar border-bottom na barra superior

### Estilização CSS - Área Principal

- [X] Centralizar verticalmente e horizontalmente o conteúdo
- [X] Aplicar tamanho grande (48px) na mensagem de boas-vindas
- [X] Estilizar campo de entrada com fundo cinza claro arredondado
- [X] Adicionar sombra sutil no campo de entrada
- [X] Alinhar botões de ação dentro do campo de entrada

### Funcionalidade e Interatividade

- [X] Adicionar estados de hover em todos os botões
- [X] Implementar transições suaves (0.2s) nos elementos interativos
- [X] Garantir que o campo de entrada seja focável
- [X] Testar acessibilidade com atributos aria-label

### Refinamentos e Detalhes

- [X] Ajustar espaçamentos (padding e margin) para corresponder ao design
- [X] Verificar alinhamento de todos os ícones
- [X] Garantir consistência de bordas arredondadas
- [X] Adicionar sombras sutis onde apropriado
- [X] Validar cores com a imagem original

### Qualidade do Código

- [X] Código HTML bem indentado e organizado
- [X] Código CSS bem estruturado e comentado
- [X] Uso adequado de classes semânticas
- [X] Variáveis CSS definidas e utilizadas consistentemente
- [X] Remover código não utilizado

---

## 🎨 Dicas de Implementação

### 1. **Estrutura de Layout**

- Use `display: flex` no body para criar o layout de duas colunas (sidebar + conteúdo)
- A sidebar deve ter largura fixa (`280px`) e o conteúdo principal deve usar `flex: 1`
- Use `flex-direction: column` dentro da sidebar para empilhar os elementos

### 2. **Cores e Estilos**

- **Cinza claro da sidebar**: `#f8f9fa`
- **Azul do Google (links e título)**: `#1a73e8`
- **Texto primário**: `#202124`
- **Texto secundário**: `#5f6368`
- **Fundo do input**: `#f1f3f4`
- **Borda**: `#dadce0`

### 3. **Tipografia**

- Família de fontes: `'Google Sans', 'Roboto', Arial, sans-serif`
- Tamanho da mensagem de boas-vindas: `48px`
- Tamanho padrão de texto: `14px`
- Logo "Gemini": `22px`

### 4. **Bordas Arredondadas**

- Botões gerais: `border-radius: 20-24px`
- Campo de entrada: `border-radius: 32px`
- Botões circulares: `border-radius: 50%`

### 5. **Efeitos Hover**

- Usar `background-color: #e8eaed` no hover
- Adicionar `transition: all 0.2s` para suavizar animações
- Sombras sutis: `box-shadow: 0 1px 2px rgba(0, 0, 0, 0.1)`

### 6. **Ícones**

- Você pode usar emojis Unicode no código inicial
- Para uma versão mais profissional, use Google Material Icons
- Alternativamente, use Font Awesome para os ícones

### 7. **Responsividade**

- Em telas menores que 768px, esconda a sidebar por padrão
- Reduza o tamanho da mensagem de boas-vindas
- Oculte textos de botões, mantendo apenas os ícones
- Ajuste paddings e margins

---

## 🚀 Desafios Extras (Opcional)

Depois de completar a réplica básica, experimente:

1. **Responsividade** usando flex
2. **Menu Hambúrguer Funcional**: Implemente JavaScript para abrir/fechar a sidebar em mobile
3. **Ícones Profissionais**: Substitua emojis por Google Material Icons ou Font Awesome
4. **Dark Mode**: Crie uma versão com tema escuro
5. **Animações**: Adicione animações de entrada nos elementos
6. **Campo de Input Expansível**: Faça o campo de entrada crescer ao focar
7. **Dropdown Funcional**: Implemente o dropdown "2.5 Pro" com opções
8. **Histórico Interativo**: Adicione mais interações ao clicar nas conversas recentes
9. **Tooltips**: Adicione tooltips nos ícones ao passar o mouse
10. **Teclado Virtual**: Simule a abertura de um teclado virtual ao clicar no campo
11. **Transições de Página**: Adicione transições suaves entre estados

---

## 📚 Recursos Úteis

### Documentação

- [MDN Web Docs - Flexbox](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Flexible_Box_Layout)
- [MDN Web Docs - CSS Grid](https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_Grid_Layout)
- [CSS Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [Google Material Design](https://material.io/design)

### Ferramentas

- [Google Fonts](https://fonts.google.com/) - Para usar a fonte Roboto
- [Material Icons](https://fonts.google.com/icons) - Ícones oficiais do Google
- [Font Awesome](https://fontawesome.com/) - Biblioteca alternativa de ícones
- [ColorZilla](https://www.colorzilla.com/) - Extensão para capturar cores
- [Chrome DevTools](https://developer.chrome.com/docs/devtools/) - Para inspecionar elementos

### Validadores

- [W3C HTML Validator](https://validator.w3.org/)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)

---

## ❓ Perguntas Frequentes

**Q: Preciso fazer a interface funcionar completamente?**
A: Não, esta atividade foca apenas na reprodução visual. Funcionalidades JavaScript são opcionais.

**Q: Posso usar frameworks CSS como Bootstrap ou Tailwind?**
A: Recomenda-se fazer com CSS puro para praticar os conceitos, mas frameworks são permitidos.

**Q: Como obtenho as cores exatas da interface?**
A: Use ferramentas como ColorZilla ou DevTools do navegador. As cores principais estão listadas nas dicas.

**Q: Preciso usar os mesmos textos das conversas recentes?**
A: Sim, replique os textos visíveis na imagem gemini.png.

**Q: E se não conseguir ícones iguais aos do Google?**
A: Use emojis Unicode inicialmente. Depois pode melhorar com Material Icons ou Font Awesome.

**Q: Como faço para validar meu trabalho?**
A: Compare visualmente com a imagem original, use validadores W3C e teste em diferentes navegadores.

**Q: Posso adicionar elementos que não estão na imagem?**
A: Para a entrega principal, mantenha fidelidade ao original. Elementos extras são bem-vindos nos desafios opcionais.

---

## 📝 Observações Importantes

- **Foco na Aparência**: Esta atividade prioriza a aparência visual sobre a funcionalidade
- **Detalhes Importam**: Preste atenção em espaçamentos, tamanhos de fonte e cores
- **Responsividade é Essencial**: Certifique-se de que funciona bem em mobile
- **Código Limpo**: Mantenha o código organizado e bem comentado
- **Use a Imagem de Referência**: Sempre compare seu trabalho com `gemini.png`

---

**Boa sorte com sua réplica! Esta é uma excelente oportunidade para praticar layout moderno e atenção aos detalhes. 💻✨**

*Atividade desenvolvida para a disciplina de Web Design - IFRN.*
