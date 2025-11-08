# Atividade: Criando Tabelas em HTML5 com Estilização

## Objetivo

Aprender a criar e estilizar tabelas em HTML5 utilizando CSS para apresentar informações de forma organizada e visualmente atraente.

## Descrição da Atividade

Você deve criar uma tabela em HTML5 que apresente informações sobre disciplinas de um curso. A tabela deve conter três colunas:

- **Disciplina**: Nome da disciplina
- **Tecnologias**: Ferramentas e tecnologias utilizadas
- **Conceitos**: Conceitos principais abordados

## Exemplo: Disciplina de Web Design

Abaixo está um exemplo completo de como criar e estilizar a tabela para a disciplina de Web Design.

### Código HTML

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tabela de Disciplinas</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Disciplinas do Curso</h1>
  
    <table>
        <thead>
            <tr>
                <th>Disciplina</th>
                <th>Tecnologias</th>
                <th>Conceitos</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Web Design</td>
                <td>
                    <ul>
                        <li>HTML</li>
                        <li>CSS</li>
                        <li>JavaScript</li>
                        <li>GitHub</li>
                        <li>VS Code</li>
                    </ul>
                </td>
                <td>
                    <ul>
                        <li>Controle de versão de código</li>
                        <li>Design de interfaces</li>
                    </ul>
                </td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```

### Código CSS (style.css)

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f4f4f4;
    padding: 20px;
}

h1 {
    text-align: center;
    color: #333;
    margin-bottom: 30px;
}

table {
    width: 100%;
    max-width: 1000px;
    margin: 0 auto;
    background-color: white;
    border-collapse: collapse;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    overflow: hidden;
}

thead {
    background-color: #4CAF50;
    color: white;
}

th {
    padding: 15px;
    text-align: left;
    font-size: 16px;
    font-weight: bold;
}

tbody tr {
    border-bottom: 1px solid #ddd;
}

tbody tr:hover {
    background-color: #f5f5f5;
}

td {
    padding: 15px;
    vertical-align: top;
}

td ul {
    list-style-position: inside;
    margin-left: 10px;
}

td ul li {
    padding: 5px 0;
    color: #555;
}

/* Responsividade para dispositivos móveis */
@media screen and (max-width: 768px) {
    table {
        font-size: 14px;
    }
  
    th, td {
        padding: 10px;
    }
}
```

## Instruções para Realizar a Atividade

- [X] **Crie um arquivo HTML** chamado `disciplinas.html`
- [X] **Crie um arquivo CSS** chamado `disciplinas.css`
- [X] **Crie a estrutura inicial do HTML 5** no arquivo `disciplinas.html`
- [X] **Defina o título da página** coloque a identificação no arquivo `disciplinas.html`. Lembre de atualizar também o `title`.
- [X] **Copie o código CSS** fornecido acima para o arquivo `disciplinas.css`
- [X] **Abra o arquivo HTML** em seu navegador para visualizar a tabela
- [X] **Experimente modificar** as cores, tamanhos e estilos para personalizar sua tabela
- [X] **Adicione as disciplinas**: matemática discreta, programação de computadores , e sistemas digitais

## Desafios Adicionais (Opcional)

- Adicione mais disciplinas à tabela (por exemplo: Programação, Banco de Dados, etc.)
- Implemente cores alternadas nas linhas da tabela usando `nth-child`
- Adicione ícones ao lado das tecnologias
- Crie uma versão responsiva que transforme a tabela em cards em dispositivos móveis

## Critérios de Avaliação

- ✅ Tabela criada com as três colunas solicitadas
- ✅ Utilização correta das tags HTML5 para tabelas (`table`, `thead`, `tbody`, `tr`, `th`, `td`)
- ✅ Estilização CSS aplicada adequadamente
- ✅ Código organizado e bem formatado
- ✅ Tabela responsiva e visualmente atraente

## Recursos Úteis

- [MDN Web Docs - Tabelas HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element/table)
- [W3Schools - HTML Tables](https://www.w3schools.com/html/html_tables.asp)
- [CSS Tricks - A Complete Guide to the Table Element](https://css-tricks.com/complete-guide-table-element/)

---

**Boa sorte com sua atividade!** 🚀
