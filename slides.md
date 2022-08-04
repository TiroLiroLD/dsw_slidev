---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://d1csarkz8obe9u.cloudfront.net/posterpreviews/blank-landscape-template-c46374b637e36ef134762358d24a5847_screen.jpg?ts=1561679189

# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Promise based HTTP client for the browser and node.js
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
---

<h1>Axios</h1>

<h2>Cliente HTTP baseado em Promises</h2>

<div class="nomes">
  <h3>Leone Crespo Daher de Souza</h3>
  <h3>Paulo Henrique Marques Madeira</h3>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
h2 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
h3 {
  background-color: #FFFFFF;
  background-size: 100%;
  text-align: right;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
.nomes {
    position: absolute;
    bottom: 0rem;
    right: 0rem;}
</style>
---

# Para que serve o Axios?

Axios é um cliente HTTP baseado em Promises para fazer requisições. 
É isomórfico, podendo portanto rodar no navegador e no node.js com a mesma base de código, e possui as seguintes características destacadas em sua própria documentação:

- Faz XMLHttpRequests do navegador
- Faz requisições http do node.js
- Suporta a API de Promises
- Intercepta requisições e respostas
- Transforma os dados de requisições e de respostas
- Cancela requisições
- Transformação de dados para JSON
- Suporta proteções contra XSRF no lado do cliente

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---

# Instalação 

É possível instalar facilmente o Axios utilizando um gestor de pacotes .js, como o npm e o yarn:

- **npm**:
<code>$ npm install axios</code>

- **Yarn**:
<code>$ yarn add axios</code>

<style>
code {
    -webkit-font-smoothing: initial;
    background-color: #f8f8f8;
    border-radius: 2px;
    color: #33333c;
    display: block;
    font-family: Roboto Mono, Monaco, Consolas, monospace;
    line-height: inherit;
    margin: 0 2px;
    max-width: inherit;
    overflow: inherit;
    padding: 2.2em 5px;
    white-space: inherit;
    font-size: 0.8em;
}
</style>

---

# Uso

Utilizando o Axios para fazer uma operação GET a uma API por um usuário 12345:

```ts {all|1|2-7|8-11|12-14|all}
const axios = require('axios');
// Faz uma requisição a um usuarío com um ID expecifico
axios.get('/user?ID=12345')
  .then(function (response) {
    // manipula o sucesso da requisição
    console.log(response);
  })
  .catch(function (error) {
    // manipula erros da requisição
    console.error(error);
  })
  .then(function () {
    // sempre será executado
  });
```
---

# Slidev

[Documentations](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev) · [Showcases](https://sli.dev/showcases.html)

# Axios

[Documentations](https://axios-http.com/ptbr/docs/) 