# exerjavascript

Atividade 1
<!DOCTYPE html>
<html>
<head>
<title> 
</title> 
<meta charset="utf-8">
</head> 
<body> 
    <h2>Exibir um alert</h2>
    <input type="button" value="Exibir alert" onclick=exibeAlert()>

<script>
    function exibeAlert(){
        alert("alert!");
    }
</script>
</body> 
</html>     

Atividade 2
<!DOCTYPE html>
<html>
<head>
<title>Tutorial de Alert em JavaScript - Linha de Código</title>
<script>
function funcao1()
{
alert("Eu sou um\nAlert!");
}
</script>
</head>
<body>

<input type="button" onclick="funcao1()" value="Exibir Alert" />

</body>
</html>

Atividade 3
O QUE É DOM?
A sigla Dom significa Document Object Model, que em português significa Modelo de Documento por Objetos. Trata-se de uma interface de programação que os navegadores utilizam para representar páginas na web. O DOM oferece um modelo de representação e interação do documento HTML ou XML. Existem alguns tipos de códigos que envolvem o DOM, que são eles:
. document.getElementById();
GetElementById como o próprio nome já diz, é uma função do JavaScript que serve para retornar um elemento do DOM que é identificado com um ID específico.
A função busca e retorna o elemento através de seu identificador, a propriedade ID, servindo para obter um elemento a partir do seu atributo ID especificado.
var elem = document.getElementById("nome-identificador");
 . document.getElementsByTagName();
O método getElementsByName() do objeto document é usado quando precisamos obter uma lista (coleção NodeList ou matriz) de elementos HTML que possuem o mesmo valor para sua propriedade name.
Você escolhe o nome para a Tag, e o programa busca as p´partes que estiverem de acordo com o que foi digitado.
var elems = document.getElementsByName("linguagens");
.document.getElementsByClassName();
Este script nos permite selecionar conjuntos de elementos do documento com base nos identificadores que estão em seu atributo class.
A função retorna um Nodelist contendo todos os descendentes coincidentes do documento ou elemento.
var elementos = document.getElementByClassName("nome-da-classe");
.document.querySelector();
O método querySelector( ) retorna o primeiro elemento filho que corresponda a um ou mais seletores CSS especificados. Para retornar todas as correspondências, use o método querySelectorAll();
document.querySelector(“CSS selectors”);
.document.querySelectorAll();
Representando uma lista de elementos do documento que correspondem ao grupo especificado de seletores, a função document.querySelectorAll recebe um argumento de string contendo um seletor CSS e retorna um objeto NodeList representando os elementos do documento que correspondem ao seletor.


Atividade 4 
EVENTOS DO JAVASCRIPT
O QUE SÃO EVENTOS?

Os eventos são basicamente um conjunto de ações que são realizadas em um determinado elemento da página web, seja ele um texto, uma imagem, ou uma div, por exemplo. Muitas das interações do usuário que está visitando sua página com o conteúdo do seu site podem ser consideradas eventos.

ONMOUSEOVER e ONMOUSEOUT

Sua tradução literal é “quando o mouse tiver por cima”, no caso, ele detecta a ação do mouse quando ela estiver sobre um determinado elemento da página.
Um exemplo é de que você pode colocar uma imagem em uma página e quando colocar o cursor em cima, ela muda, porém, quando o mouse não estiver mais sobre ela, no caso, a imagem voltará a seu estado normal.
<!DOCTYPE html>
<html>
<head>
<title>Usando eventos no Javascript</title>
</head>
<body>

<div onmouseover="mOver(this)" onmouseout="mOut(this)"
style="background-color:#D94A38;width:120px;height:20px;padding:40px;">Passe o mouse em mim</div>

<script>
function mOver(obj)
{
obj.innerHTML="Obrigado"
}

function mOut(obj)
{
obj.innerHTML="Passe o mouse em mim"
}
</script>

</body>
</html>

ONFOCUS e ONBLUR

O evento onfocus dispara quando algum tipo de formulário (como input) está selecionado, ou seja, quando estamos usando-o, clicamos, digitamos ou estamos exercendo alguma ação nele. Já o evento onblur ocorre quando 'saímos' desse formulário. Exemplo:

function dentro ()
{
   document.getElementById("meuInput").style.background = "red";
}

function fora()
{
   document.getElementById("meuInput").style.background = "blue” }

ONCHANGE
O evento onchange é utilizado para que seja realizada determinada ação após alguma mudança. No exemplo abaixo iremos fazer essa mudança acontecer ao clicarmos fora do texto input.
<!DOCTYPE html>
<html>
<head>
<title>Usando eventos no Javascript</title>
<script>
function myFunction()
{
var x=document.getElementById("fname");
x.value=x.value.toUpperCase();
}
</script>
</head>
<body>

Insira seu Nome: <input type="text" id="fname" onchange="myFunction()">
<p>
Ao clicarmos fora do input text o texto escrito nele ficará todo em caixa alta.</p>

</body>
</html>




EVENTOS DO JAVASCRIPT
O QUE SÃO EVENTOS?

Os eventos são basicamente um conjunto de ações que são realizadas em um determinado elemento da página web, seja ele um texto, uma imagem, ou uma div, por exemplo. Muitas das interações do usuário que está visitando sua página com o conteúdo do seu site podem ser consideradas eventos.

ONMOUSEOVER e ONMOUSEOUT

Sua tradução literal é “quando o mouse tiver por cima”, no caso, ele detecta a ação do mouse quando ela estiver sobre um determinado elemento da página.
Um exemplo é de que você pode colocar uma imagem em uma página e quando colocar o cursor em cima, ela muda, porém, quando o mouse não estiver mais sobre ela, no caso, a imagem voltará a seu estado normal.
<!DOCTYPE html>
<html>
<head>
<title>Usando eventos no Javascript</title>
</head>
<body>

<div onmouseover="mOver(this)" onmouseout="mOut(this)"
style="background-color:#D94A38;width:120px;height:20px;padding:40px;">Passe o mouse em mim</div>

<script>
function mOver(obj)
{
obj.innerHTML="Obrigado"
}

function mOut(obj)
{
obj.innerHTML="Passe o mouse em mim"
}
</script>

</body>
</html>

ONFOCUS e ONBLUR

O evento onfocus dispara quando algum tipo de formulário (como input) está selecionado, ou seja, quando estamos usando-o, clicamos, digitamos ou estamos exercendo alguma ação nele. Já o evento onblur ocorre quando 'saímos' desse formulário. Exemplo:

function dentro ()
{
   document.getElementById("meuInput").style.background = "red";
}

function fora()
{
   document.getElementById("meuInput").style.background = "blue” }

ONCHANGE
O evento onchange é utilizado para que seja realizada determinada ação após alguma mudança. No exemplo abaixo iremos fazer essa mudança acontecer ao clicarmos fora do texto input.
<!DOCTYPE html>
<html>
<head>
<title>Usando eventos no Javascript</title>
<script>
function myFunction()
{
var x=document.getElementById("fname");
x.value=x.value.toUpperCase();
}
</script>
</head>
<body>

Insira seu Nome: <input type="text" id="fname" onchange="myFunction()">
<p>
Ao clicarmos fora do input text o texto escrito nele ficará todo em caixa alta.</p>

</body>
</html>

atividade 5
FUNÇÃO NOMEADA
Você irá criar uma função nomeada quando quiser reutilizar ela em vários 
pontos do seu código.
NOTAÇÂO LITERAL
A maneira mais simples de se criar objetos em Javascript é chamado de notação 
literal. Que é composto por um par de chaves “{}", que envolve uma ou mais 
propriedades. Cada propriedade segue um formato "nome: valor" e devem ser 
separadas por vírgula.
1. var album = {
2. title: "Metallica (Black Album)",
3. released: 1991,
4. showInfo: funcion () {
5. alert ("Título do álbum: " + this.title + "Lançado em: " +
this.released);
6. }
7. };
FUNÇÃO DE FLEXA
Arrow functions se destaca. Elas não possuem um this.
constructor(){
this.list = [];
this.pushArray();
}
pushArray(){
let newList = [1, 2, 3];
newList.forEach(function(value) {
this.list.push(value);
});
console.log(this.list);
 }
FUNÇÃO NOMEADA
Você irá criar uma função nomeada quando quiser reutilizar ela em vários 
pontos do seu código.
NOTAÇÂO LITERAL
A maneira mais simples de se criar objetos em Javascript é chamado de notação 
literal. Que é composto por um par de chaves “{}", que envolve uma ou mais 
propriedades. Cada propriedade segue um formato "nome: valor" e devem ser 
separadas por vírgula.
1. var album = {
2. title: "Metallica (Black Album)",
3. released: 1991,
4. showInfo: funcion () {
5. alert ("Título do álbum: " + this.title + "Lançado em: " +
this.released);
6. }
7. };
FUNÇÃO DE FLEXA
Arrow functions se destaca. Elas não possuem um this.
constructor(){
this.list = [];
this.pushArray();
}
pushArray(){
let newList = [1, 2, 3];
newList.forEach(function(value) {
this.list.push(value);
});
console.log(this.list);
 }
FUNÇÃO NOMEADA
Você irá criar uma função nomeada quando quiser reutilizar ela em vários 
pontos do seu código.
NOTAÇÂO LITERAL
A maneira mais simples de se criar objetos em Javascript é chamado de notação 
literal. Que é composto por um par de chaves “{}", que envolve uma ou mais 
propriedades. Cada propriedade segue um formato "nome: valor" e devem ser 
separadas por vírgula.
1. var album = {
2. title: "Metallica (Black Album)",
3. released: 1991,
4. showInfo: funcion () {
5. alert ("Título do álbum: " + this.title + "Lançado em: " +
this.released);
6. }
7. };
FUNÇÃO DE FLEXA
Arrow functions se destaca. Elas não possuem um this.
constructor(){
this.list = [];
this.pushArray();
}
pushArray(){
let newList = [1, 2, 3];
newList.forEach(function(value) {
this.list.push(value);
}
console.log(this.list);
 }

