# exerjavascript
FUNÇÃO NOMEADA
Você irá criar uma função nomeada quando quiser reutilizar ela em vários pontos do seu código.

var math = {
  'factorial': function factorial(n) {
    if (n <= 1)
      return 1;
    return n * factorial(n - 1);
  }
};


FUNÇÃO CONSTRUTORA
As funções construtoras são como as classes do Java, diferenciando apenas pela sintaxe. Em questão de funcionamento, tanto funções construtoras no Javascript quanto Classes no Java têm a mesma utilidade: servir de molde para a criação de objetos.
Para construir objetos, funções construtoras precisam ser instanciadas pelo operador new. O this dentro delas se referência ao objeto criado a partir delas.
No exemplo abaixo, a função Carro é uma função construtora, e carro1 é um objeto criado a partir do “molde” dessa classe, usando o operador new:

Function Carro (marca, modelo, ano) {
	this.marca = marca
	this.modelo = modelo
	this.ano = ano
}

const carro1 = new Carro (‘Charger’, ‘RT’,  ‘1970)
 console.log = (carro1)


NOTAÇÂO LITERAL
A maneira mais simples de se criar objetos em Javascript é chamado de notação literal. Que é composto por um par de chaves “{}", que envolve uma ou mais propriedades. Cada propriedade segue um formato "nome: valor" e devem ser separadas por vírgula.

   var album = {
	  title: "Metallica (Black Album)",
	  released: 1991,
	  showInfo: funcion () {
	    alert ("Título do álbum: " + this.title + "Lançado em: " + this.released);
	  }
};


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
}

