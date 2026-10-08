# 💻 Portfólio — João Pedro

Portfólio pessoal desenvolvido utilizando **HTML5 e CSS3**, com foco em apresentar informações pessoais, habilidades, projetos e formas de contato de maneira moderna, organizada e responsiva.

---

## 📌 Sobre o projeto

Este projeto consiste em um site de portfólio pessoal para **João Pedro**.

O objetivo é apresentar, de forma profissional, informações sobre o desenvolvedor, suas habilidades e seus projetos.

O site foi desenvolvido utilizando apenas:

* HTML5
* CSS3

Não foram utilizados frameworks ou bibliotecas JavaScript.

---

## 📁 Estrutura do projeto

```text
portfolio/
│
├── index.html
├── style.css
└── README.md
```

### `index.html`

Responsável pela **estrutura e conteúdo** da página.

Nele estão presentes:

* Cabeçalho
* Menu de navegação
* Seção inicial
* Seção "Sobre mim"
* Seção de habilidades
* Seção de projetos
* Seção de contato
* Rodapé

### `style.css`

Responsável pela **aparência visual** do site.

O arquivo controla:

* Cores
* Tipografia
* Espaçamentos
* Tamanhos
* Posicionamento
* Bordas
* Efeitos de hover
* Responsividade
* Layout das seções

---

# 🏗️ Estrutura HTML

O projeto utiliza HTML5 semântico para organizar o conteúdo.

### `<header>`

Contém o cabeçalho e o menu principal do site.

```html
<header>
    <nav class="navbar">
        ...
    </nav>
</header>
```

O menu possui links que levam diretamente para as seções da página.

Exemplo:

```html
<a href="#projetos">Projetos</a>
```

O `#projetos` aponta para:

```html
<section id="projetos">
```

Dessa forma, o usuário consegue navegar pelas diferentes partes do portfólio.

---

## 🏠 Seção inicial

A seção inicial apresenta as principais informações do portfólio.

Ela contém:

* Nome
* Área de atuação
* Pequena descrição
* Botão para projetos
* Botão de contato
* Elemento visual com símbolo de código

Estrutura:

```html
<section id="inicio" class="inicio">
```

Essa seção funciona como a apresentação inicial do usuário.

---

# 👤 Seção "Sobre mim"

A seção apresenta informações sobre João Pedro.

Ela utiliza dois cards:

```html
<div class="sobre-card">
```

Um card apresenta informações sobre quem é o usuário e o outro apresenta seus objetivos.

---

# 🛠️ Seção de habilidades

A seção de habilidades apresenta as principais tecnologias e conhecimentos.

Atualmente estão cadastradas:

* HTML
* CSS
* Web Design
* Git

Cada habilidade possui um card próprio.

Exemplo:

```html
<div class="habilidade">
    <h3>HTML</h3>
    <p>Estruturação de páginas web.</p>
</div>
```

---

# 📂 Seção de projetos

A seção de projetos apresenta trabalhos desenvolvidos.

Cada projeto utiliza um elemento:

```html
<article class="projeto">
```

Cada card possui:

* Número do projeto
* Nome
* Descrição
* Tecnologias utilizadas
* Link do projeto

Exemplo:

```html
<article class="projeto">
    <div class="projeto-numero">01</div>

    <h3>Site Educacional</h3>

    <p>
        Plataforma de estudos criada para organizar
        matérias, materiais e atividades.
    </p>
</article>
```

---

# 📧 Seção de contato

A seção de contato permite que o visitante envie uma mensagem por e-mail.

Foi utilizado o protocolo:

```html
mailto:
```

Exemplo:

```html
<a href="mailto:seuemail@email.com">
    Enviar mensagem
</a>
```

Para utilizar um e-mail real, basta substituir:

```text
seuemail@email.com
```

pelo endereço desejado.

---

# 🎨 Desenvolvimento CSS

O arquivo `style.css` foi dividido em diferentes partes para facilitar a manutenção.

A organização utilizada é:

```text
Configurações gerais
        ↓
Navbar
        ↓
Seção inicial
        ↓
Elemento visual
        ↓
Seções
        ↓
Sobre
        ↓
Habilidades
        ↓
Projetos
        ↓
Contato
        ↓
Rodapé
        ↓
Responsividade
```

---

# 🎨 Paleta de cores

O projeto utiliza principalmente um tema escuro.

### Fundo principal

```css
#0b0f19
```

Utilizado como fundo principal da página.

### Fundo secundário

```css
#0e1420
```

Utilizado para diferenciar algumas seções.

### Cor de destaque

```css
#6c63ff
```

Utilizada em:

* Botões
* Links
* Títulos secundários
* Detalhes dos cards
* Logo
* Elementos de destaque

### Texto principal

```css
#ffffff
```

Utilizado nos títulos e textos de maior importância.

### Texto secundário

```css
#9299aa
```

Utilizado para descrições e informações complementares.

---

# 🔤 Tipografia

O projeto utiliza a fonte:

```css
Poppins
```

A fonte é carregada através do Google Fonts:

```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
```

A Poppins foi escolhida por possuir um estilo moderno e adequado para interfaces e portfólios.

---

# 📐 Layout

O projeto utiliza principalmente **Flexbox** e **CSS Grid**.

## Flexbox

Utilizado no menu:

```css
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
```

Também é utilizado na seção inicial para posicionar o conteúdo e o elemento visual.

---

## CSS Grid

Utilizado para organizar cards.

Exemplo:

```css
.projetos-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
}
```

Isso cria três colunas para os projetos em telas maiores.

---

# 🖱️ Efeitos de interação

O projeto utiliza `transition` e `transform` para criar pequenas animações quando o usuário passa o mouse sobre determinados elementos.

Exemplo:

```css
.projeto:hover {
    transform: translateY(-8px);
    border-color: #6c63ff;
}
```

Quando o mouse passa sobre um projeto, ele sobe levemente e sua borda muda de cor.

Também existem efeitos nos botões:

```css
.botao:hover {
    background: #554de0;
    transform: translateY(-3px);
}
```

---

# 📱 Responsividade

O site foi desenvolvido para funcionar em diferentes tamanhos de tela.

Foram utilizadas **Media Queries**.

Exemplo:

```css
@media (max-width: 900px) {
    ...
}
```

Para telas menores, o layout dos elementos é reorganizado.

Em celulares, por exemplo, os projetos passam de três colunas para uma:

```css
.projetos-grid {
    grid-template-columns: 1fr;
}
```

Também existe uma configuração específica para telas com até `650px` de largura.

```css
@media (max-width: 650px) {
    ...
}
```

---

# 🔗 Navegação interna

A navegação utiliza âncoras HTML.

Exemplo:

```html
<a href="#sobre">Sobre</a>
```

O link aponta para:

```html
<section id="sobre">
```

O CSS também utiliza:

```css
scroll-behavior: smooth;
```

Isso faz com que a página role suavemente até a seção selecionada.

---

# 🚀 Como executar o projeto

Não é necessário instalar nenhum programa ou dependência.

### 1. Baixe ou copie os arquivos

```text
index.html
style.css
README.md
```

### 2. Coloque os arquivos na mesma pasta

```text
portfolio/
├── index.html
├── style.css
└── README.md
```

### 3. Abra o arquivo

Abra:

```text
index.html
```

com qualquer navegador moderno, como:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Opera

---

# ✏️ Como personalizar

## Alterar o nome

No `index.html`, procure:

```html
<h2>João Pedro</h2>
```

e altere para o nome desejado.

---

## Alterar habilidades

Procure:

```html
<div class="habilidade">
    <h3>HTML</h3>
    <p>Estruturação de páginas web.</p>
</div>
```

Você pode adicionar novas habilidades copiando esse bloco.

---

## Adicionar projetos

Para adicionar outro projeto, copie:

```html
<article class="projeto">
    ...
</article>
```

e altere as informações.

---

## Alterar o e-mail

Procure:

```html
href="mailto:seuemail@email.com"
```

e coloque seu endereço de e-mail.

---

# 🧰 Tecnologias utilizadas

| Tecnologia    | Utilização                |
| ------------- | ------------------------- |
| HTML5         | Estrutura do site         |
| CSS3          | Estilização               |
| Flexbox       | Organização dos elementos |
| CSS Grid      | Layout dos cards          |
| Media Queries | Responsividade            |
| Google Fonts  | Tipografia                |

---

# 📈 Possíveis melhorias futuras

O projeto pode ser expandido futuramente com:

* JavaScript
* Formulário de contato funcional
* Animações mais avançadas
* Modo claro/escuro
* Página individual para cada projeto
* Integração com GitHub
* Download de currículo
* Área de certificados
* Foto de perfil
* Mais projetos
* Backend para armazenamento de mensagens

---

# 👨‍💻 Autor

**João Pedro**

Portfólio pessoal desenvolvido para apresentar conhecimentos, projetos e evolução na área de desenvolvimento web.

---

## 📄 Licença

Este projeto foi desenvolvido para uso pessoal e educacional.
