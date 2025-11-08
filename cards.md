# Atividade: Lista de Cards em HTML5

## 📋 Objetivo da Atividade

Criar uma lista de cards estilizados em HTML5 que apresentem informações sobre disciplinas. Cada card deve conter três seções principais: **título**, **conteúdo** e **rodapé**.

## 🎯 Estrutura do Card

Cada card deve ter:

### 1. **Título (Header)**

- Nome da disciplina
- Nome do(s) professor(es)

### 2. **Conteúdo (Content)**

- Objetivo da disciplina
- Carga horária
- Tecnologias utilizadas
- Conceitos abordados

### 3. **Rodapé (Footer)**

- Horários das aulas
- Salas/laboratórios utilizados

---

## 💻 Exemplo: Disciplina de Web Design

### Informações da Disciplina

**Disciplina:** Web Design
**Professores:** Danielle Freitas e Leonardo Minora

**Objetivo:**
Capacitar os alunos no desenvolvimento de interfaces web modernas e responsivas, utilizando as principais tecnologias e boas práticas de desenvolvimento front-end.

**Carga horária:** 80 horas

**Tecnologias:**

- HTML
- CSS
- JavaScript
- GitHub
- VS Code

**Conceitos:**

- Controle de versão de código
- Design de interfaces

**Horários:**

- Segunda-feira: 14h00 às 18h00 - Laboratório 6
- Terça-feira: 14h00 às 18h00 - Laboratório 6

---

## 📝 Instruções para Implementação

### Passo 1: Estrutura HTML

Crie um arquivo `index.html` com a estrutura básica do HTML5:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cards de Disciplinas</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1>Disciplinas Ofertadas</h1>
      
        <!-- Card da disciplina -->
        <div class="card">
            <!-- Título do Card -->
            <div class="card-header">
                <h2>Web Design</h2>
                <p class="professores">Prof. Danielle Freitas e Prof. Leonardo Minora</p>
            </div>
          
            <!-- Conteúdo do Card -->
            <div class="card-content">
                <h3>Objetivo</h3>
                <p>Capacitar os alunos no desenvolvimento de interfaces web modernas e responsivas, utilizando as principais tecnologias e boas práticas de desenvolvimento front-end.</p>
              
                <h3>Carga Horária</h3>
                <p>80 horas</p>
              
                <h3>Tecnologias</h3>
                <ul class="tecnologias">
                    <li>HTML</li>
                    <li>CSS</li>
                    <li>JavaScript</li>
                    <li>GitHub</li>
                    <li>VS Code</li>
                </ul>
              
                <h3>Conceitos</h3>
                <ul class="conceitos">
                    <li>Controle de versão de código</li>
                    <li>Design de interfaces</li>
                </ul>
            </div>
          
            <!-- Rodapé do Card -->
            <div class="card-footer">
                <h3>Horários e Locais</h3>
                <p><strong>Segunda-feira:</strong> 14h00 às 18h00 - Laboratório 6</p>
                <p><strong>Terça-feira:</strong> 14h00 às 18h00 - Laboratório 6</p>
            </div>
        </div>
      
    </div>
</body>
</html>
```

### Passo 2: Estilização CSS

Crie um arquivo `styles.css` para estilizar os cards:

```css
/* Reset básico */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    padding: 20px;
    line-height: 1.6;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
}

.container h1 {
    text-align: center;
    color: #333;
    margin-bottom: 30px;
    font-size: 2.5em;
}

/* Estilo do Card */
.card {
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    margin-bottom: 30px;
    overflow: hidden;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 12px rgba(0, 0, 0, 0.15);
}

/* Header do Card */
.card-header {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 20px;
    text-align: center;
}

.card-header h2 {
    font-size: 2em;
    margin-bottom: 10px;
}

.card-header .professores {
    font-size: 1.1em;
    font-style: italic;
    opacity: 0.9;
}

/* Conteúdo do Card */
.card-content {
    padding: 25px;
}

.card-content h3 {
    color: #667eea;
    margin-top: 15px;
    margin-bottom: 10px;
    font-size: 1.3em;
}

.card-content p {
    color: #555;
    margin-bottom: 15px;
}

.card-content ul {
    list-style: none;
    padding-left: 0;
}

.card-content ul li {
    background-color: #f0f0f0;
    padding: 8px 12px;
    margin-bottom: 8px;
    border-left: 4px solid #667eea;
    border-radius: 4px;
}

.tecnologias li {
    display: inline-block;
    background-color: #667eea;
    color: white;
    padding: 6px 15px;
    margin: 5px;
    border-radius: 20px;
    border-left: none;
    font-size: 0.9em;
}

/* Rodapé do Card */
.card-footer {
    background-color: #f9f9f9;
    padding: 20px;
    border-top: 2px solid #e0e0e0;
}

.card-footer h3 {
    color: #333;
    margin-bottom: 10px;
    font-size: 1.2em;
}

.card-footer p {
    color: #666;
    margin-bottom: 8px;
}

.card-footer strong {
    color: #667eea;
}

/* Responsividade */
@media (max-width: 768px) {
    .container h1 {
        font-size: 2em;
    }
  
    .card-header h2 {
        font-size: 1.5em;
    }
  
    .tecnologias li {
        display: block;
        margin: 5px 0;
    }
}
```

---

## 🎨 Desafios Extras

Depois de implementar o card básico, tente os seguintes desafios:

1. **Múltiplos Cards**: Adicione mais cards de diferentes disciplinas
2. **Grid Layout**: Organize os cards em uma grade usando CSS Grid ou Flexbox
3. **Animações**: Adicione animações suaves ao passar o mouse sobre os cards
4. **Ícones**: Utilize bibliotecas de ícones (como Font Awesome) para ilustrar as tecnologias
5. **Dark Mode**: Implemente um botão para alternar entre modo claro e escuro
6. **Filtros**: Adicione botões para filtrar cards por categoria ou tecnologia
7. **Busca**: Implemente uma barra de busca para encontrar disciplinas

---

## ✅ Checklist de Entrega

- [X] Arquivo `index.html` criado com a estrutura correta
- [X] Arquivo `styles.css` criado com estilização adequada
- [X] Card contém título com nome da disciplina e professores
- [X] Card contém conteúdo com objetivo, carga horária, tecnologias e conceitos
- [X] Card contém rodapé com horários e locais
- [X] Design é responsivo e funciona em diferentes tamanhos de tela
- [X] Código está bem indentado e organizado
- [X] Projeto está versionado no GitHub

---

## 📚 Recursos Adicionais

- [MDN Web Docs - HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
- [MDN Web Docs - CSS](https://developer.mozilla.org/pt-BR/docs/Web/CSS)
- [CSS Tricks - Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [CSS Tricks - Grid Guide](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Google Fonts](https://fonts.google.com/)
- [Font Awesome Icons](https://fontawesome.com/)

---

## 🎓 Critérios de Avaliação

- **Estrutura HTML (30%)**: Uso correto das tags HTML5 semânticas
- **Estilização CSS (30%)**: Cards bem estilizados e visualmente agradáveis
- **Responsividade (20%)**: Layout adaptável para diferentes dispositivos
- **Organização do Código (10%)**: Código limpo, indentado e bem comentado
- **Criatividade (10%)**: Implementação de recursos extras e personalização

---

**Boa prática e bons estudos! 🚀**
