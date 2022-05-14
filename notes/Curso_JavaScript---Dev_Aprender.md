# Curso JavaScript - DevAprender

[Link do curso](https://www.youtube.com/watch?v=i6Oi-YtXnAU&t=9157s)

**camelCase** → primeira palavra em minúsculo e as palavras seguintes com a primeira letra em maiúsculo.

**PascalCase** → sempre a primeira letra de todas as palavras são maiúsculas.

**Tipos primitivos:**

- String literal;
- Number literal;
- Boolean;
- Undefined;
- null → redefinir um valor.

**typeof** → definife o tipo primitivo da variável.

**Operador tenário**

```javascript
var idade = readlineSync.question("Digite sua idade: ")
let maioridade = idade >= 18 ? 'Maior de idade!' : 'Menor de idade!'
console.log("===================")
console.log(maioridade)
```

```shell
var idade = readlineSync.question("Digite sua idade: ")
let maioridade = idade >= 18 ? 'Maior de idade!' : 'Menor de idade!'
console.log("===================")
console.log(maioridade)
```

**Falsy:**

- ​	undefined
- ​	null
- ​	0
- ​	false
- ​	‘’
- ​	NaN – not a number

**Truthy:**

- ​	valores que não são falsy.

**Factory Functions** → **Funções de Fábrica**: Criando objetos de forma dinâmica.

```javascript
console.log('---------------------------------------')
console.log(' factoryFunctions → Funções de Fábrica ')
console.log('---------------------------------------')
function criarCelular(marcaCelular, tamanhoTela, capaciadeBateria){
	return {
		marcaCelular,
		tamanhoTela,
		capaciadeBateria,
		ligar(){
			console.log('Fazendo ligação...')
		}
	}
}
let marca = readlineSync.question('Qual a marca do celular: ')
let tamanho = Number(readlineSync.question('Qual o tamanho da tela: '))
let bateria = Number(readlineSync.question('Qual a capacidade da bateria: '))
console.log(criarCelular(marca, tamanho, bateria))
console.log('---------------------------------------')
```

```shell
---------------------------------------
 factoryFunctions → Funções de Fábrica 
---------------------------------------
Qual a marca do celular: nokia
Qual o tamanho da tela: 6
Qual a capacidade da bateria: 3000mA
{
  marcaCelular: 'nokia',
  tamanhoTela: 6,
  capaciadeBateria: NaN,
  ligar: [Function: ligar]
}
---------------------------------------
```

**Constructor Functions** → **Função de Construtor**: tem como objetivo realizar a mesma tafera da Factory Functions, porém de um jeito diferente.

**this.propriedade** → serve para referenciar o objeto.

```javascript
console.log('----------------------------------------------')
console.log(' Constructor Functions → Função de Construtor ')
console.log('----------------------------------------------')
function Celular(marcaCelular, tamanhoTela, capacidadeBateria){
	this.marcaCelular = marcaCelular,
	this.tamanhoTela = tamanhoTela,
	this.capacidadeBateria = capacidadeBateria,
	this.ligar = function(){
		console.log('fazendo ligação...')
	}
}
let marca = readlineSync.question('Qual a marca do celular: ')
let tamanho = Number(readlineSync.question('Qual o tamanho da tela: '))
let bateria = Number(readlineSync.question('Qual a capacidade da bateria: '))
console.log(new Celular(marca, tamanho, bateria))
console.log('----------------------------------------------')
```

```shell
----------------------------------------------
 Constructor Functions → Função de Construtor 
----------------------------------------------
Qual a marca do celular: samsung
Qual o tamanho da tela: 5.4
Qual a capacidade da bateria: 6000mA
Celular {
  marcaCelular: 'samsung',
  tamanhoTela: 5.4,
  capacidadeBateria: NaN,
  ligar: [Function (anonymous)]
}
----------------------------------------------
```

**Natureza dinâmica de objetos:**

```javascript
console.log('Objeto original:')
const mouse = {
	cor: 'red',
	marcar: 'dazz',
}
console.log(mouse)

console.log('-------------------')
console.log('Adicionando Propriedades:')
mouse.velocidade = 5000
mouse.trocarDPI = function () {
	console.log('mudando DPI')
}
console.log(mouse)

console.log('-------------------')
console.log('Deletando Propriedades:')
delete mouse.velocidade
delete mouse.trocarDPI
console.log(mouse)
```

```shell
Objeto original:
{ cor: 'red', marcar: 'dazz' }
-------------------
Adicionando Propriedades:
{
  cor: 'red',
  marcar: 'dazz',
  velocidade: 5000,
  trocarDPI: [Function (anonymous)]
}
-------------------
Deletando Propriedades:
{ cor: 'red', marcar: 'dazz' }
```

**Clonando Objetos**: 

```javascript
const celular = {
	marcaCelular: 'ASUS',
	tamanhoTela:{
		vertivcal: 155,
		horizontal: 75
	},
	ligar: function () {
		console.log('Fazendo ligação...')
	}
}
console.log('-------------------')
console.log('Objeto original')
console.log('-------------------')
console.log(celular)
console.log('-------------------')
console.log('Clonando Objeto!') // Object.assign
console.log('-------------------')
const novoObjeto = Object.assign({
	bateria: 5000
}, celular)
console.log(novoObjeto)
console.log('-------------------')
console.log('Clonando Objeto!') // ...
console.log('-------------------')
const objeto2 = {...celular}
console.log(objeto2)
```

```shell
-------------------
Objeto original
-------------------
{
  marcaCelular: 'ASUS',
  tamanhoTela: { vertivcal: 155, horizontal: 75 },
  ligar: [Function: ligar]
}
-------------------
Clonando Objeto!
-------------------
{
  bateria: 5000,
  marcaCelular: 'ASUS',
  tamanhoTela: { vertivcal: 155, horizontal: 75 },
  ligar: [Function: ligar]
}
-------------------
Clonando Objeto!
-------------------
{
  marcaCelular: 'ASUS',
  tamanhoTela: { vertivcal: 155, horizontal: 75 },
  ligar: [Function: ligar]
}
```

**Math:**

- Math.**random** -> gera um número aleatório entre 0 e 1

```javascript
console.log(Math.random())
```

```shell
0.3412602771200346
```

- Math.**max** -> retorna o maior valor de um intervalo de valore passado para a função.

```javascript
console.log(Math.max(3,6,15,8,10))
```

```shell
15
```

- Math.**min** -> retorna o menor valor de um intervalo de valore passado para a função.

```javascript
console.log(Math.min(3,6,15,2,8,10))
```

```shell
2
```

**String:**

- Tipo primitivo

```javascript
const mensagem = ' minha primeira mensagem '
```

- Tipo Objeto

```javascript
const outraMensagem = new String('bom dia')
```

- length -> informa a quantidade de caracteres da string.

```javascript
console.log(outraMensagem.length)
```

```shell
7
```

- acessando um caracter a partir do **índice**.

```javascript
console.log(outraMensagem[2])
```

```shell
m
```

- procurando algum caracter ou palavra dentro da string.

```javascript
console.log(mensagem.includes('primeira'))
```

```shell
true
```

- procurando pelo caracter ou palavra que a string começa.

```javascript
console.log(mensagem.startsWith('minha'))
```

```shell
false
```

- procurando pelo caracter ou palavra que a string termina.

```javascript
console.log(mensagem.endsWith('mensagem'))
```

```shell
false
```

- para saber qual o índice de algum caracter ou palavra dentro da string.

```javascript
console.log(mensagem.indexOf('primeira'))
```

```shell
7
```

- replace para substituir um termo dentro da string.

```javascript
console.log(mensagem.replace('minha', 'sua'))
```

```shell
 sua primeira mensagem 
```

- para remover os espaço excedentes no início e no final da string.

```javascript
console.log(mensagem.trim())
```

```shell
minha primeira mensagem
```

- para separar o conteúdo da string.

```javascript
console.log(mensagem.split(' '))
```

```shell
[ '', 'minha', 'primeira', 'mensagem', '' ]
```

**Template literal:**

```javascript
const mensagem = 
'Oi isso é a minha\n' +
'\'primeira\' mensagem'
console.log(mensagem)
```

```shell
Oi isso é a minha
'primeira' mensagem
```

```javascript
// Object {}
// Boolean true,false
// string '', ""
// Template ``
const outra = `oi isso é a minha
'primeira' mensagem`
console.log(outra)
```

```shell
oi isso é a minha
'primeira' mensagem
```



```javascript
const nome = 'Thiago'
const email = 
`ola ${nome}

Obrigado por se inscrever no canal

Para acompanhar os vídeos não se esqueça de ativar o sino.

Obrigado,
Bill.`
console.log(email)
```

```shell
ola Thiago

Obrigado por se inscrever no canal

Para acompanhar os vídeos não se esqueça de ativar o sino.

Obrigado,
Bill.
```

**Date:**

```javascript
const data1 = new Date()
console.log(data1)
```

```shell
2022-05-14T22:48:55.583Z
```

``` javascript
const data2 = new Date('septembre 06 2022 07:30')
console.log(data2)
```

```shell
2022-09-06T10:30:00.000Z
```

```javascript
const data3 = new Date(2022,08,27,7,30)
console.log(data3)
```

```shell
2022-09-27T10:30:00.000Z
```

```javascript
console.log(data1.toDateString()) // para apresentar como string.
console.log(data1.toTimeString()) // para apresentar o padrão.
console.log(data1.toISOString()) // como visualiza no banco de dados.
```

```shell
Sat May 14 2022
19:53:52 GMT-0300 (Horário Padrão de Brasília)
2022-05-14T22:53:52.325Z
```

**Introdução a Arrays:**

- Adicionar novos elementos;
- Encontrar elementos;
- Remover elementos;
- Dividir elementos;
- Dividir Arrays;
- Combinar Arrays.

**Adicionar elementos a um Arrays:**

```javascript
let numeros = [1, 2, 3]
console.log(`Array Original: ${numeros}`)
```

```shell
Array Original: 1,2,3
```

- **Início**

```javascript
numeros.unshift(0)
console.log(`Array add início: ${numeros}`)
```

```shell
Array add início: 0,1,2,3
```

- **Meio**

```javascript
numeros.splice(1, 0, 'a') // o 1ª parâmetro é o índice onde será add o novo valor. O 2º parâmetro é o que você quer deletar e o 3º é o que será inserido.
console.log(`Array add no meio: ${numeros}`)
```

```shell
Array add no meio: 0,a,1,2,3
```

- **Final**

```javascript
numeros.push(5)
console.log(`Array add final: ${numeros}`)
```

```shell
Array add final: 0,a,1,2,3,5
```

**Encontrando um elemento:**PAREI

- **Primitivos:**

**indexOf** → retorna o índice do valor procurado dentro do array. Caso o valor não seja encontrado, será retornado -1.

```javascript
const numeros = [1, 2, 3, 1, 4]
console.log(numeros.indexOf(1))
```

**lastIndexOf** → retorna o índice da última ocorrência daquele valor procurado dentro do array.

```javascript
console.log(numeros.lastIndexOf(1))
```

**includes** → retorna true ou false se o valor procurado existir dentro do array.

```javascript
console.log(numeros.includes(2))
```

- **Referência:**

```javascript
const marcas =[
	{id:1, nome: 'a'},
	{id:2, nome: 'b'}
]
const marca = marcas.find(function(marca){
	return marca.nome === 'b'
})
console.log(marca)
```

- **Arrow Functions:**

```javascript
const marcas = [
	{id:1, nome: 'a'},
	{id:2, nome: 'b'}
]
const marca = marcas.find(marca => marca.nome = 'c')
console.log(marca)
```

- **Removendo Elementos do array:**

```javascript
const alfabeto = ['a', 'b', 'c', 'd', 'e', 'f']
console.log(`Array Original: ${alfabeto}`)
// Final
const ultimo = alfabeto.pop()
console.log(`Último elemento: ${ultimo}`)
console.log(`Após remover último elemento: ${alfabeto}`)
// Início
const primeiro = alfabeto.shift()
console.log(`Primeiro elemento: ${primeiro}`)
console.log(`Após remover 1º elemento: ${alfabeto}`)
// Meio
const meio = alfabeto.splice(2,1)
console.log(`Elemento do meio: ${meio}`)
console.log(`Após remover elemento do meio: ${alfabeto}`)
```

- **Esvaziando um Array:**

```javascript
let letras = ['a', 'b', 'c', 'd', 'e', 'f']
let outras = letras
console.log(`Array letras: ${letras}`)
console.log(`Array outras: ${outras}`)
```

**1ª solução:** não recomendada

```javascript
letras = []
console.log('1º solução:')
console.log(`Array letras: ${letras}`)
console.log(`Array outras: ${outras}`)
```

**2ª solução:** melhor solução

```javascript
letras.length = 0
console.log('2º solução:')
console.log(`Array letras: ${letras}`)
console.log(`Array outras: ${outras}`)
```

**3ª solução:**

```javascript
letras.splice(0, letras.length)
console.log('3º solução:')
console.log(`Array letras: ${letras}`)
console.log(`Array outras: ${outras}`)
```

**4ª solução:** requer muito do sistema em grandes bancos de dados.

```javascript
while(letras.length > 0){
	letras.pop()
}
console.log('4º solução:')
console.log(`Array letras: ${letras}`)
console.log(`Array outras: ${outras}`)
```

- **Combinar Arrays:**

```javascript
const primeiro = ['a', 'b', 'c']
const segundo = ['d', 'e', 'f']
const combinado = primeiro.concat(segundo)
console.log(`1º array: ${primeiro}`)
console.log(`2º array: ${segundo}`)
console.log(`Arrays juntos: ${combinado}`)
```

- **Dividir Array:**

```javascript
const primeiro = ['a', 'b', 'c']
const segundo = ['d', 'e', 'f']
const combinado = primeiro.concat(segundo)
console.log(`1º array: ${primeiro}`)
console.log(`2º array: ${segundo}`)
console.log(`Arrays juntos: ${combinado}`)
const cortado = combinado.slice(1, 3)
console.log(`Array a partir do índice 1 até o índice 2: ${cortado}`)
const cortado = combinado.slice(1) // inicia a partir do índice passado até o último índice
console.log(`Array a partir do índice passado: ${cortado}`)
const cortado = combinado.slice() // copia todo o array
console.log(cortado)
```

- **Operador Spread**

```javascript
const primeiro = ['a', 'b', 'c']
const segundo = ['d', 'e', 'f']
const combinado = [...primeiro, ...segundo]
const combinado2 = [...primeiro, 1, ...segundo, '%']
const clonado = [...combinado]
console.log('Primeiro: '+primeiro)
console.log(`Segundo: ${segundo}`)
console.log(`Combinado: ${combinado}`)
console.log(`Combinado 2: ${combinado2}`)
console.log(`Clonado: ${clonado}`)
```

- **forEach**

```javascript
const letras = ['a', 'b', 'c', 'd', 'e', 'f']
console.log("for of")
for(indice of letras){
	console.log(indice)
}
console.log("forEach")
letras.forEach((letras, indice) => console.log(`Letras: ${letras} - Índice: ${indice}`))
```

```shell
for of
a
b
c
d
e
f
forEach
Letras: a - Índice: 0
Letras: b - Índice: 1
Letras: c - Índice: 2
Letras: d - Índice: 3
Letras: e - Índice: 4
Letras: f - Índice: 5
```

- **Combinando Arrays**

```javascript
const letras = ['a', 'b', 'c', 'd', 'e', 'f']
const combinado = letras.join('.')
const frase = 'Estou aprendendo JavaScript com DevAprender'
const resultado = frase.split(' ')
console.log(letras)
console.log(combinado)
console.log(frase)
console.log(resultado)
console.log(resultado.join('-'))
```

```shell
[ 'a', 'b', 'c', 'd', 'e', 'f' ]
a.b.c.d.e.f
Estou aprendendo JavaScript com DevAprender
[ 'Estou', 'aprendendo', 'JavaScript', 'com', 'DevAprender' ]
Estou-aprendendo-JavaScript-com-DevAprender
```

- **Recebendo Dados (INPUT)**

```javascript
let name = prompt("What's your name?")
alert(`Welcome ${name}`)
let age = Number(prompt("What's your age?"))
alert(age >= 18 ? `Ok ${name}, você tem ${age} anos e é maior de idade!`: `Ok ${name}, você tem ${age} anos e é menor de idade!`)
```

![promptA](/home/thiagocarlos/Imagens/promptA.png)

![promptB](/home/thiagocarlos/Imagens/promptB.png)

![promptC](/home/thiagocarlos/Imagens/promptC.png)

![promptD](/home/thiagocarlos/Imagens/promptD.png)

- **Intro Manipulação do DOM**

**Exercícios:**

**ex001_trocandoValores** → Crie um programa que troque os valores das variáveis apresentadas abaixo:

```javascript
let a = "vermelho"
let b = 'azul'
console.log(a)
console.log(b)
```

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex001_trocandoValores.js)

**ex002_horaDoDia** → Elabore um programa em que de acordo com a hora do dia ele exiba uma mensagem de acordo com as instruções abaixo:

```tex
Se a hora estiver entre 06:00 até 12:00 → Bom dia!
Se estiver entre 12:00 até 18:00 → Boa tarde!
Caso contrátio → Boa noite!
```

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex002_horaDoDia.js)

**ex003_maiorNumero** → Escreva uma função que usa dois números e retorna o maior entre eles.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex003_maiorNumero.js)

**ex004_Fizzbuzz** → Desenvolva um programa que tenha uma função em que seja inserido um valor e se o valor for divisível por 3, retorne “Fizz”; Se o valor for divisível por 5, retorne “Buzz”; Se o valor for divisível por 3 e 5, retorne “FizzBuzz”; Se o valor não é divisível por 3 ou por 5, retorne o valor inserido; E se o valor inserido não é um número, retornar a mensagem “não é um número”.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex004_Fizzbuzz.js)

**ex005_medidorDeVelocidade** → Faça um programa que simule os radares de velocidade de trânsito. Considere a velocidade máxima como sendo 70km/h. A cada 5km acima do limite, o motorista ganha 1 ponto na carteira. Use a função Math.floor( ).

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex005_medidorDeVelocidade.js)

**ex006_parOuImpar** → Crie um programa em que receba uma quantidade de valores para avaliar. A função exibe se cada valor é par ou ímpar.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex006_parOuImpar.js)

**ex007_encontreOString** → Elabore um programa para ler propriedades de um objeto e exibir somente as propriedades do tipo string que estão nesse objeto.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex007_encontreOString.js)

**ex008_somaMultiplos** → Desenvolva um programa em que seja inserido um valor e ele retorne a soma de todos os múltiplos de 3 e de 5 dentro daquele valor.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex008_somaMultiplos.js)

**ex009_mediaNotaEscolar** → Faça um programa que receba notas de alunos. Essas notas devem ser amazenadas em um array. O programa deve calcular a média das notas e de acordo com a tabela a seguir, deve dizer qual foi o conceito da turma a partir da sua média.

| **0 		→ 59**   | **F** |
| -------------------- | ----- |
| **60 		→ 69**  | **D** |
| **70 		→ 79**  | **C** |
| **80 		→ 89**  | **B** |
| **90 		→ 100** | **A** |

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex009_mediaNotaEscolar.js)

**ex010_exibirAsteriscos** → Crie um programa que exibe a quantidade de * que aquela linha possui.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex010_exibirAsteriscos.js)

**ex011_numerosPrimos** → Elabore uma função em que o usuário passe para ela um limite e a função vai percorer todos os números desse limite e dizer quais desse números são primos ou não. O programa deve mostar na tela os números primos.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex011_numerosPrimos.js)

**ex012_montadorDeEndereco** → Desenvolva um programa que tenha um objeto endereço. Nesse objeto deve ser adicionado a rua, cidade, CEP. Crie uma função exibirEndereco para exibir todas as propriedades do objeto e seus valores.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex012_montadorDeEndereco.js)

**ex013_encontreAIgualdade** → Faça um programa que tenha dois objetos. Esse programa deve ter uma função que faça comparação entre as suas propriedades e o endereço de memória.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex013_encontreAIgualdade.js)

**ex014_montadorPostagemBlog** → Crie um programa que tenha um objeto de postagem de blog que vai conter as seguintes propriedades: título, mensagem, autor, visulizações, comentários[array] (autor, mensagem), está ao vivo.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex014_montadorPostagemBlog.js)

**ex015_constructorFunction** → Elabore um programa que tenha um objeto postagem usando uma função de construtor que tenha as seguintes informações: título, mensagem, autor, vizualizações, Array de comentários, e se está ao vivo ou não.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex015_constructorFunction.js)

**ex016_faixaDePreco** → Construa um programa que tenha um array de objetos de faixa de preços para que ela possa ser usada em um site igual o mercado livre. O array será chamado de faixas, e terá como propriedade tooltip, valor mínimo e valor máximo.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex016_faixaDePreco.js)

**ex017_segurançaVirtual** → Elabore um programa em que o usuário informe seu nome e o programa verifique se o nome do usuário está numa lista pré-determinada de convidados ou não. Caso o nome do usuário esteja na lista, a mensagem “Você pode entrar!” deve ser apresentada, caso contrário, a mensagem “Você não pode entrar!” deve ser apresentada.

Resposta - [clique aqui](https://github.com/tthiagocarlosdev/TESTES/blob/main/Curso%20JavaScript%20DevAprender/ex017_seguran%C3%A7aVirtual.js)

**Desafio final - segurançaVirtual:**

Crie uma página HTML que tenha como título “Festa VIP” e dois campos para pegar nomes e um botão! O 1º campo deve pegar o nome do usuário e o 2º campo o nome de quem o convidou para a festa. Depois de preencher os dois campos o usuário deve clicar no botão “Verificar se posso entrar”. Abaixo será exibido um mensagem. Caso seu nome esteja na lista, altere a descrição “Pesquisando...” para “Você pode entrar!”. Caso seu nome não esteja na lista a descrição de “Pesquisando...” altera para “Você não pode entrar!”. Segue abaixo o modelo da página HTML para ajudar!

  ![img](file:///tmp/lu159623695x2.tmp/lu159623695x9_tmp_17e42fd98a459117.png) 

Resposta - [clique aqui]()