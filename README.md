<h1>Elementos do DOM</h1>
<h2>Instruções do projeto</h2>
<p>Crie um projeto com dois arquivos: index.html e script.js. 
  No arquivo 'index' insira a estrutura base HTML e dentro da tag 'body' inclua quatro tags vazias: h1, ul, a, ol. 
  Adicione o atributo id="titulo" à tag h1, o atributo href="https://prozeducacao.com.br" à tag 'a', e o atributo id="lista-ordenada" à tag 'ol'. 
  Na sequência, realize a conexão entre o arquivo HTML e o arquivo JavaScript.
</p>
<p>
No arquivo script.js capture os quatro elementos criados, e use a propriedade 
  .innerText para adicionar conteúdo textual aos elementos 'h1' e 'a', e a propriedade 
  .innerHTML para adicionar três itens simples na lista não ordenada, e três itens com links para outros sites na lista ordenada. 
</p>

<h3>Código html</h3>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manipulando propriedades com o DOM</title>
    <script src="./script.js" defer></script>
</head>
<body>
    <h1 id="titulo"></h1>
    <a href="https://prozeducacao.com.br"></a>
    <ol id="lista-ordenada"></ol>
    <h2></h2>
    <ul></ul>    
</body>
</html>
```
<h3>Código javascript</h3>

```
const titulo = document.querySelector("#titulo");
titulo.innerText = "Proz";

const link = document.querySelector("a");
link.innerText = "Nosso site";

const listaOrdenada = document.querySelector("#lista-ordenada");
listaOrdenada.innerHTML = `
    <li><a href="#">Quem somos</a></li>
    <li><a href="#">Cursos</a></li>
    <li><a href="#">Unidades</a></li>
`;

const h2 = document.querySelector("h2");
h2.innerText = "Serviços";

const listaNaoOrdenada = document.querySelector("ul");
listaNaoOrdenada.innerHTML = `
    <li>Curso técnico</li>
    <li>Curso de capacitação</li>
    <li>Preparaçao para certificação</li>
`;
```
