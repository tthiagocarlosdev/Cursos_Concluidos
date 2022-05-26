# Curso de JavaScript - Curso em Vídeo - 2848

Professor: Gustavo Guanabara

[Link do Curso](https://www.youtube.com/watch?v=1-w1RfGIov4&list=PLHz_AreHm4dlsK3Nr9GVvXCbpQyHQl1o1)

## Aula 04 – Criando o seu primeiro script

- **window.alert** – Para exibir uma janela com uma mensagem:

```javascript
window.alert('Minha primeira mensagem')
```

- **window.confirm** – Para exibir uma janela com uma pergunta:

```javascript
window.confirm('Está gostando de JS?')
```

- **window.prompt** – Para exibir uma janela para o usuário preencher com texto:

```javascript
window.prompt('Qual é seu nome?')
```

## Aula 05 – Variáveis e Tipos Primitivos

- **Comentários no JavaScript:**

Os comentários são utilizados para ajudar a entender o código em consultas porteriores.

- **//** - Para única linha:

```javascript
// única linha
```

- **/\* \*/** - Para mais de uma linha de código:

```javascript
/*

comentário em

mais de 

uma linha

*/
```

- **Variáveis:**

Variáveis servem para guardar dados. Podem ser do **tipo inteiro** (5, 18, -12); **tipo real/float** (0.5, -15.9, 3.14, 8.0); OBS.: No JavaScript os tipos inteiro e real são considerados apenas um tipo, o **number;** Podem ser do tipo **string**, que são cadeias de caracteres (“Google”, ‘JavaScript’, 'Maria', “12345”); e por fim podem ser do tipo **Boolean** (true, false).

Outros tipos:

O **Number** também apresenta os tipos **Infinity** e **NaN**. Temos também os tipos **null**, **undefined**, **object**, **array**, **function**.

- **$ typeof** – Para identificar de qual tipo é a sua variável.

No JavaScript moderno, além de utilizar a palavra **var**, também podemos usar a palavra **let**. O símbolo **=** é denominado “**recebe**”. Por exemplo.:

**var s1 = carro** – significa que a variável s1 está **recebendo** o valor carro.

Para declarar **strings** podemos fazer das seguintes maneiras:

var s1 = **“**JavaScript**” - entre aspas duplas.**

var s2 = **‘**Curso em Vídeo**’ - entre aspas simples.**

var s3 = \`Guanabara` - **entre crases.**

- **Identificador** – nome de cada variável.

- **Regras para nomear identificadores:**
  - Podem começar com **letra**, **$** ou **_**
  - Não podem começar com números
  - É possível usar letras ou números
  - É possível usar acentos e símbolos
  - Não podem conter espaços
  - Não podem ser palavras reservadas

- **Dicas importantes:**
  - Maiúsculas e minúsculas fazem a diferença (case sensitive);
  - Tente escolher nomes coerentes para as variáveis;
  - Evite se tornar um programador alfabeto ou um programador contador;

## Aula 06 – Tratamentos de dados

- **Data Types:**
  - number
  - string

O símbolo de **+** é utilizado tanto para somar em operações como para **concatenar** diferentes tipos de variáveis.

**window.prompt** retorna uma **string**.

- **Convertendo tipos de dados:**
  - **String → Número:**

    - **Number.parseInt(n)** – Converte para número inteiro;
    - **Number.parseFloat(n)** – Converte para número real/float.

```javascript
var numero1 = Number.parseInt(window.prompt("Digite um número: "))
var numero2 = Number.parseInt(window.prompt("Digite outro número: "))
```

Esse dois comandos são usados para forçar a converção para **Inteiro** ou **Float**. Mas usando apenas **Number.** A variável será convertida para algum tipo de número e o próprio **JS** vai determinar se será **Inteiro** ou **Float**.

```javascript
var numero1 = Number(window.prompt("Digite um número: "))
var numero2 = Number(window.prompt("Digite outro número: "))
```

- **Número → String:**
  - **String(n)** - Para converter para string.
  - **n.toString()** - Para converter para string.

```javascript
window.alert("A soma entre os valores é igual a "+String(soma)) // Concatenação
```

- **Formatando Strings:**

```javascript
var s = ‘JavaScript’
‘Eu estou aprendendo s’ // não faz interpolação
‘Eu estou aprendendo ’ + s // usa concatenação
`Eu estou aprendendo ${s}` // usa template string
```

```javascript
window.alert(`A soma entre ${numero1} e ${numero2} é igual a ${soma}`)
```

- **s.length** // informa quantos caracteres a string tem:

```javascript
document.write(`Olá <strong>${nome}</strong>. Seu nome tem ${nome.length} letras.<br/>`)
```

- **s.toUpperCase( )** // tudo para ‘MAIÚSCULAS’:

```javascript
document.write(`Seu nome em maiúsculo: ${nome.toUpperCase()}<br/>`)
```

- **s.LowerCase( )** // tudo para ‘minúsculas’:

```javascript
document.write(`Seu nome em minúsculo: ${nome.toLocaleLowerCase()}<br/>`)
```

- **Formatando Números:**

var n = 1541.5

**n.toFixed(2)** – Para formatar o número apresentando com a quantidade de casas decimais informada dentro do parênteses, nesse caso, duas casas decimais:

**.replace(‘’, ‘’)** - Troca o que está dentro do primeiro parâmetro pelo o que está no segundo.

**Find out the proper way to replace all occurrences of a string in plain JavaScript, from regex to other approaches** - [link](https://flaviocopes.com/how-to-replace-all-occurrences-string-javascript/)

**n.toFixed(2).replace(‘.’, ‘,’)** - nesse caso trocará o ponto pela vírgula.

**Para converter o número para moeda:**

- Real:

```javascript
n.toLocaleString('pt-BR', {style: 'currency', currency: 'BRL'})
```

```shell
R$ 1.541,50
```

- Dólar:

```javascript
n.toLocaleString('pt-BR', {style: 'currency', currency: 'USD'})
```

```shell
US$ 1.541,50
```

- Euro:

```javascript
n.toLocaleString('pt-BR', {style: 'currency', currency: 'EUR'})
```

```shell
€ 1.541,50
```

## Aula 07 – Operadores (Parte 1) 

**Tipos de Operadores:**

- Aritméticos;
- Atribuição;
- Relacionais;
- Lógicos;
- Ternário.

### Aritméticos (binários):

5 **+** 2 = 7 **→  Soma**

5 **-** 2 = 3 **→ Subtração**

5 ***** 2 = 10 **→ Multiplicação**

5 **/** 2 = 2.5 **→ Divisão real**

5 **%** 2 = 1 **→ Divisão inteira**

5 ***\*** 2 = 25 **→ Potência**

Cuidado com a **ordem de precedência** dos operadores, é a mesma da matemática.

**1º → ( )**

**2º → \****

**3º → \* / %**

**4º → + -**

###  Atribuição:

| **Auto-atribuições** | **Auto-atribuições** |
| :------------------: | :------------------: |
|      **Normal**      |   **Simplificada**   |
|      var n = 3       |                      |
|  n = n + 4 **→** 7   |  n += 4 → 		7  |
|  n = n – 5 **→** 2   |  n -= 5 → 		2  |
|  n = n * 4 **→** 8   |  n *= 4 → 		8  |
|  n = n / 2 **→** 4   |  n /= 2 → 		4  |
|   n = n ** 2 → 16    | n **= 2 → 		16 |
|    n = n % 5 → 1     |  n %= 5 → 		1  |

|    **Incremento**     | **Incremento** |
| :-------------------: | :------------: |
|       var x = 5       |                |
|     x = x + 1 → 6     |      x++       |
| x = x – 1 → 		5 |      x--       |

## Aula 08 - Operadores (Parte 2)

### Relacionais:

Para toda expressão que tenha um operador relacional a ela, o seu resultado será sempre um valor booleano.

5 > 2 → true

7 < 4 → false

8 >= 8 → true

9 <= 7 → false

5 == 5 → true

4 != 4 → false

### Relacionais de Identidade:

**Indêntico** → mesmo valor e mesmo tipo.

5 == 5 → true

5 == ‘5’ → true

5 === ‘5’ → false

5 === 5 → true

5 != 5 → false

5 != ‘5’ → false

5 !== ‘5’ → true

5 !== 5 → false

### Lógicos:

**! → negação (não) → operador unário.**

| !true  | false |
| :----: | :---: |
| !false | true  |

**&& → conjunção (e) → operador binário.**

|  true && true  | true  |
| :------------: | :---: |
| true && false  | false |
| false && true  | false |
| false && false | false |

**|| → disjunção (ou) → operador binário.**

|  true \|\| true  | True  |
| :--------------: | :---: |
| true \|\| false  | True  |
| false \|\| true  | True  |
| false \|\| false | false |

**Ordem de precedência dos lógicos:**

1º → não (!)

2º → e (&&)

3º → ou (||)

**Ordem de precedência dos operadores:**

1º operadores aritméticos

2º operadores relacionais

3º operadores lógicos

### Ternário:

teste **?** true **:** false

```javascript
média >= 7.0 ? “Aprovado” : “Reprovado”
```

## Aula 09 – Introdução ao DOM

Document Object Model

Árvore DOM

Manipulando DOM

### DOM → Documente Object Model:

**Modelo de objetos para documentos**. Conjunto de objetos dentro do navegador que vai dar acesso aos componentes internos do seu website. DOM não funciona dentro do Node.js. Funciona quando rodamos JavaScript dentro do navegador.

### Árvore DOM:

window – raiz do DOM. Tudo dentro do JavaScript está dentro do window.

- Window
  - location
  - document
    - html
      - head
        - meta
        - title
      - body
        - h1
        - p
        - p
          - strong
        - div
  - history

**Selecionando:** Métodos de acesso para navegar entre cada elemento da árvore DOM.

Métodos:

- **por Marca**

getElementsByTagName()

```javascript
var p1 = window.document.getElementsByTagName('p')[1]
window.document.write('Está escrito assim: '+p1.innerText)
window.document.write('Puxando a formatação: '+p1.innerHTML)
```

- **por ID**

getElementById() - Posso identificar um elemento por id e acessá=lo através do getElementByld().

```html
<div id="mensagem">Clique em mim</div>
var d = window.document.getElementById('mensagem')
d.style.background = 'purple'
```

- **por Nome**

getElementsByName() - Para acessar pelo nome do elemento.

```html
<div name="mensagem">Clique em mim</div>
var d = window.document.getElementsByName('mensagem')[0]
d.innerText = "Hello, World!"
```

- **por Classe**

getElementsByClassName()

```html
<div class="mensagem">Clique em mim</div>
var d = window.document.getElementsByClassName('mensagem')[0]
d.style.background = "pink"
```

- **por Seletor**

querySelector()

querySelectorAll()

Toda div é representada por ‘#’ e toda class é representada por ‘.’.

```html
<div id="mensagem">Clique em mim</div>
var d = window.document.querySelector('div#mensagem')
d.style.color = 'blue'
```

```html
<div class="mensagem">Clique em mim</div>
var d = window.document.querySelector('div.mensagem')
d.style.color = 'yellow'
```

## Aula 10 - Eventos DOM

Eventos DOM

Evento é tudo aquilo que pode acontecer com um elemento.

[Events](https://developer.mozilla.org/pt-BR/docs/Web/Events)

### Função:

Conjunto de códigos/linhas que vão ser executadas só quando o evento ocorrer.

**Function ação(parâmetros){ }**

```javascript
function ação(parâmetro){
	código
}
```

**Exemplo de interação no HTML:**

```html
<body>
	<div id="area" onclick="clicar()"onmouseenter="entrar()" onmouseout="sair()">
	Interaja...
	</div>
<script>
	function clicar() {
		var area = window.document.getElementById("area");
		area.innerText = "Clicou"
		area.style.background = "red"
	}
	function entrar(){
		var area = window.document.getElementById("area");
		area.innerText = "Entrou!"
	}
	function sair(){
		var area = window.document.getElementById("area");
		area.innerText = "Saiu!!"
		area.style.background = "green"
	} 
</script>
</body>
```

**Exemplo de interação no próprio JavaScript:**

```html
<body>
	<div id="area">
		Interaja...
	</div>
<script>
	var area = window.document.getElementById("area");
	area.addEventListener("click", clicar)
	area.addEventListener("mouseenter", entrar)
	area.addEventListener("mouseout", sair)
	function clicar() {
		area.innerText = "Clicou"
		area.style.background = "red"
	}
	function entrar(){
		area.innerText = "Entrou!"
	}
	function sair(){
		area.innerText = "Saiu!!"
		area.style.background = "green"
	} 
</script>
</body>
```

**Detectando erros**:

Ao executar um código e perceber que ele não funcionou do jeito programado, você pode clicar com o botão direito do mouse na página e clicar em **inspencionar**. Irá abrir o **DevTools** e no final do **DevTools**, na aba **console** será apresentado o erro e aonde está acontecendo.

## Aula 11 – Condições (Parte 1)

### Sequências

```javascript
var n = 2
n += 2
window.alert(n)
```

### Condições

```javascript
if (condição){
	true
} else {
	false
}
```

### Tipos de Condição

- **Condição simples**

```javascript
if (condição){
	true
}
```

- **Condição composta**

```javascript
if (condição){
	true
} else {
	false
}
```

```javascript
var idade = 17
if(idade < 18){
	console.log('Menor de idade!')
} else {
	console.log('Maior de idade!')
}
```

## Aula 12 - Condições (Parte 2)

- **Condição Aninhada**

```javascript
if(condição1){
	bloco 1
} else {
	if(condição 2){
		bloco 2
	} else {
		bloco 3
	}
}
```

```javascript
var idade = 66
console.log(`Você tem ${idade} anos.`)
if(idade < 16){
	console.log('Não vota!')
} else if (idade < 18 || idade > 65){
	console.log('Voto opcional!')
} else {
	console.log('Voto obrigatório')
}
```

```javascript
var agora = new Date()
var hora = agora.getHours()
var minutos = agora.getMinutes()
var segundos = agora.getSeconds()
console.log(`Agora são exatamente ${hora}h${minutos}min${segundos}seg.`)
if (hora < 12) {
	console.log('Bom dia!')
} else if (hora <= 18){
	console.log('Boa tarde')
} else {
	console.log('Boa noite')
}
```

- **Condição Multipla –** usada para valores fixos.

```javascript
switch(expressão){
	case valor 1:
		bloco
	break
	case valor 2:
		bloco
	break
	case valor 3: 
		bloco
	break
	default:
		bloco
	break
}
```

```javascript
var agora = new Date()
var diaSemana = agora.getDay()
console.log(diaSemana)
switch (diaSemana) {
	case 0:
		console.log('Domingo')
	break;
	case 1:
		console.log('Segunda')
	break;
	case 2:
		console.log('Terça')
	break;
	case 3:
		console.log('Quarta')
	break;
	case 4:
		console.log('Quinta')
	break;
	case 5:
		console.log('Sexta')
	break;
	case 6:
		console.log('Sábado')
	break;
	default:
		console.log('ERRO! Dia inválido!')
	break;
}
```

## Exercícios Javascript – Parte 1

**Modelo**

**HTML**

```html
<!DOCTYPE html>
<html lang="pt-BR">
	<head>
		<meta charset="UTF-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1.0">
		<title>Modelo de Exercício</title>
		<link rel="stylesheet" href="estilo.css">
	</head>
<body>
	<header>
		<h1>Título</h1>
	</header>
	<section>
		<div>
			<p>Testando</p>
		</div>
		<div>
			<p>Hello</p>
		</div>
	</section>
	<footer>
		<p>&copy;CursoemVídeo</p>
	</footer>
	<script src="script.js"></script>
</body>
</html>
```

**CSS**

```css
body{

​	background:rgb(88, 208, 212);

​	font: normal 15pt verdana;

}

header{

​	color:white;

​	text-align: center;

}

section{

​	background:white;

​	border-radius: 10px;

​	padding: 15px;

​	width: 500px;

​	margin: 0 auto;

​	box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.609); 

}

footer{

​	color:white;

​	text-align: center;

​	font-style: italic;

}
```

## Exercícios JavaScript – Parte 2

## Exercícios JavaScript – Parte 3

## Aula 13 – Repetições – Parte 1 - PAREI

**Repetições/Laços**

**Laço “enquanto”:** **Testa a condição para depois executar o bloco/comando. Enquanto a condição for verdadeira, ele continuará a executar o bloco/comando. Estrutura de repetição com teste lógico no início.**



**while(condição){**

​	**comando**

**}**



**Exemplo:**



var computador = 1

while (computador <= 6){

​	console.log(('Tudo bem?'))

​	computador++

}





**Laço “faça”:** **Executa o bloco/comando para depois testar a condição. Enquanto a condição for verdadeira, ele continuará a executar o bloco/comando. Estrutura de repetição com teste lógico no final.**



**do{**

​	**comando**

**}while(condição)**



computador = 1

do{

​	console.log(`Passo ${computador}`)

​	computador++

}while(computador <= 6)



- ​	**Aula 14 – Repetições – Parte 2**

**Estrutura de repetição com variável de controle.**

**Laço “para”: Inicia uma variável, executa um teste e se este teste for verdadeiro, executa o bloco, volta para o início e incrementa a variável. Realiza novamente o teste e se for verdadeiro continua a executar o bloco e incrementando, até o teste ser falso.**



**for(inicialização; teste; incremento){**

​	**comando**

**}**



for(var computador = 1; computador <= 5; computador++){

​	console.log(`Passo ${computador}`)

}



- ​	**Exercícios JavaScript – Parte 4**



Demonstração dos exercícios



- ​	**Exercícios JavaScript – Parte 5**

**Para adicionar emoji no JavaScript:**

https://unicode.org/emoji/charts/full-emoji-list.html

copia o código, apenas os caracteres após o símbolo de +, e no JavaScript digita: `\u{código}`. Ex.: `\u{1F600}`.



- ​	**Exercícios JavaScript – Parte 6**



- ​	**Aula 15 – Variáveis Compostas**

**Variáveis simples** só conseguem armazenar **um valor** por vez.

**Variáveis compostas** devem ser capazes de armazenar **vários valores** em uma mesma estrutura.

**Variável composta = Array = vetor** → é uma variável que possui vários elementos, cada elemento é composto por seu valor e por uma chave de identificação (índice/chave).

Exemplo de declaração de array.:

**let numero = [5, 8, 4]**

Para acrescentar valores em um array existente:

**numero[3] = 6** → O array numero no índice 3 receberá o valor 6.

**numero.push(7)** → O array numero no próximo índice receberá o valor 7.

Para saber o tamanho do array, basta usar o atributo **length**:

**numero.length**

Para organizar todos o elementos do array em ordem crescente, basta utilizar o método **sort()**:

**numero.sort()**

Para mostrar apenas um valor de um array, basta declarar o array e entre colchetes declarar o índice do valor a ser mostrado:

**numero[0]** → irá mostrar o valor de índice zero no array.

**console.log(numero)** → para mostrar todo o seu array.

Outra forma é usando estrutura de repetição:

let valores = [3, 6, 5, 9, 1, 7, 8, 0, 10]

for (let contador = 0; contador < valores.length; contador++){

​	console.log(`A posição ${contador} tem o valor: ${valores[contador]}.`)

}



E outra forma mais simples é usado a estrutura de repetição **for in**:

for(let contador in valores){

​	console.log(`A posição ${contador} tem o valor: ${valores[contador]}.`)

}



O **for in** só funciona para objetos e arrays. Estrutura básica do **for in**:



**for(let posicao in numero){**

**console.log(`A posição ${posicao} tem o valor: ${numero[contador]}.`)**

**}**

A leitura é feita da seguinte maneira: Para cada posição em numero, realize o bloco abaixo.



**n****umero.indexOf(7)** → Para buscar um valor dentro do array. Neste caso irá buscar o valor 7 dentro do array e irá retorna a sua chave/índice. Quando o valor procurado dentro do array não existir, a pesquisa retornará -1.



- ​	**Aula 16 – Funções**

Toda função tem uma **chamada**, comando para iniciar a função, parâmetro, ação e retorno.

**Funções** **→** São **ações** executadas assim que são **chamadas** ou em decorrência de algum **evento**. Uma **função** pode receber **parâmetros** e retornar um **resultado**.

Estrutura básica:



**function ação(parâmetro formal){**

​	**bloco a ser executado → ação**

​	**return resposta → retorno**

**}**

**ação(parâmetro real) → chamada**





Exemplo:

function parImpar(numero){

​	if(numero % 2 == 0){

​		return 'Par'

​	} else {

​		return 'Impar'

​	}

}

valor = 4

console.log(`O número ${valor} é ${parImpar(valor)}!`)



Podemos também determinar o valor inicial dos parâmetros formais, caso seja passado apenas um parâmetro real, a função funcionará corretamente. Se o valor inicial dos parâmetros formais não forem determinados, a função poderá apresentar um erro, NaN.



function soma(numeroA = 0, numeroB = 0) {

​	return numeroA + numeroB

}

let resultado = soma(2)

console.log(resultado)



podemos também colocar uma função dentro de uma variável e executá-la:



let dobro = function(x) {

​	return x*2

}

console.log(dobro(6))



Outro exemplo:



function fatorial(numero){

let fat = 1

for(let contador = numero; contador > 1; contador--){

​	fat *= contador

}

​	return fat

}

console.log(fatorial(3))





- ​	**Exercícios JavaScript – Parte 7**



- ​	**Exercícios JavaScript – Parte 8**



- ​	**Próximos Passos**

Curso de HTML5 e CSS

Estudar funções

Estudar objetos

Estudar modularização

Estudar expressões regulares

Estudar JSON

Estudar AJAX

Estudar NodeJS



- ​	**Gerar números aleatórios:**

http://devfuria.com.br/javascript/numeros-aleatorios/



https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Math/random



- ​	**Mudar estilo CSS no JavaScript:**

https://www.horadecodar.com.br/2020/05/27/como-usar-javascript-para-mudar-propriedades-css/



Fala programador(a), beleza? Bora aprender a adicionar CSS com JS!



A ideia por trás dessa técnica é muito simples, primeiramente precisamos selecionar o elemento alvo



Seja por classe, id ou query selector, para isso você pode utilizar os métodos:



getElementById

getElementsByClassName

querySelector ou querySelectorAll

Feito isso você precisa acessar a propriedade style do elemento selecionado, e fazer as alterações no CSS



Lembrando que regras como background-color que tem duas palavras, você deve substituir pelo camelCase desta maneira: backgroundColor



Vamos a um exemplo prático:



**<**!DOCTYPE html**>**

**<**html**>**

**<**head**>**

​	**<**title**>**Como usar JavaScript para mudar propriedades CSS**<**/title**>**

	<meta charset="utf-8">

**<**/head**>**

**<**body**>**

	<p id="paragrafo">Este parágrafo vai ter o CSS alterado!</p>

**<**/body**>**

**<**/html**>**



Bom, aqui temos uma tag p, com um id de parágrafo, agora vamos selecionar este elemento e alterar o estilo dele com JavaScript



let el = document.getElementById**(**'paragrafo'**)**;

// alterando uma propriedade

el.style.color = 'red';

// varias propriedades

el.style.cssText =

​	'color: blue;' +

​	'background-color: yellow;' +

​	'border: 1px solid magenta';



Aqui temos duas formas de alterar CSS, uma de propriedade singular e outra de multi propriedades



A primeira opção devemos colocar cada propriedade em uma linha, o que pode ser bem custoso caso queiramos estilizar muito o componente



Já na segunda forma concatenamos uma string em várias linhas, o que da uma impressão de CSS e fica organizado, para atingir várias propriedades de uma vez só



Vai da sua escolha e necessidade



E é claro, quando uma linha de código altera uma propriedade que já tinha valor antes, a anterior é substituída ( que é o caso do color )



O elemento recebeu todos os estilos da segunda regra, e o da primeira foi substituído



E é assim que alteramos CSS com JavaScript



Conclusão



Neste artigo vimos  usar JavaScript para mudar propriedades CSS



Precisamos selecionar o elemento e depois alterar a propriedade style com a regra que queremos mudar no CSS, por exemplo border



Aí inserimos os valores e o CSS é alterado



Há a possibilidade de alterar múltiplas regras com a propriedade cssText, porém precisamos passar uma string com todas elas



- ​	**próximo tópico**

https://www.devmedia.com.br/forum/criar-botao-dinamicamente-no-javascript/554111