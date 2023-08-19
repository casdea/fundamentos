# Roteiro de Ensino de JavaScript

## Seção 1: Introdução ao JavaScript

**Conceito:** JavaScript na web e Tipagem Fraca

**Exemplo:** Variáveis em JavaScript podem ter tipos variados:
```javascript
let x = 10;       // x é um número
x = "Hello";      // x agora é uma string
x = true;         // x agora é um booleano

Seção 2: Variáveis com var, let e const
Conceito: Diferenças entre var, let, e const

var: Escopo de função ou global, permite reatribuição.
let: Escopo de bloco, permite reatribuição.
const: Escopo de bloco, não permite reatribuição (valor constante).

Exemplo:

let a = 10;
let b = 20;
const c = 30;

a = 5;   // Isso é permitido com var
b = 15;  // Isso é permitido com let
// c = 25;  // Isso gerará um erro, pois c é constante

Seção 3: Tipos de Dados em JavaScript
Number
Conceito: O tipo Number representa valores numéricos, inteiros ou de ponto flutuante.

Exemplo: Declarando e usando números em JavaScript.

let idade = 30;
let preco = 19.99;


Math
Conceito: O objeto Math fornece funções matemáticas para realizar cálculos complexos.

Exemplo: Usando o objeto Math para calcular a raiz quadrada.

let numero = 16;
let raizQuadrada = Math.sqrt(numero);
console.log(raizQuadrada); // Saída: 4

String
Conceito: O tipo String representa sequências de caracteres.

Exemplo: Declarando e manipulando strings.

let saudacao = "Olá, mundo!";
let comprimento = saudacao.length; // Retorna 12


Template String
Conceito: Template strings são strings que permitem interpolação de variáveis e quebras de linha.

Exemplo: Usando template strings para criar mensagens formatadas.

javascript

Template String
Conceito: Template strings são strings que permitem interpolação de variáveis e quebras de linha.

Exemplo: Usando template strings para criar mensagens formatadas.

javascript

Boolean
Conceito: O tipo Boolean representa valores lógicos verdadeiro (true) ou falso (false).

Exemplo: Usando booleanos em expressões lógicas.

let temPermissao = true;
let estaLogado = false;
let resultado = temPermissao && estaLogado; // Retorna false

Array
Conceito: Um array é uma coleção ordenada de valores, que podem ser de diferentes tipos.

Exemplo: Declarando e acessando elementos de um array.

let frutas = ["maçã", "banana", "laranja"];
console.log(frutas[0]); // Saída: maçã


Object
Conceito: Um objeto é uma coleção de pares chave-valor que permite armazenar e acessar dados de maneira estruturada.

Exemplo: Declarando e acessando propriedades de um objeto.

javascript

let pessoa = {
    nome: "João",
    idade: 25,
    cidade: "São Paulo"
};
console.log(pessoa.nome); // Saída: João

Null e Undefined
Conceito: null representa a ausência intencional de qualquer valor ou objeto. undefined é usado quando uma variável foi declarada, mas ainda não foi atribuída um valor.

Exemplo: Demonstrando o uso de null e undefined.

let valorNulo = null;
let valorIndefinido;
console.log(valorNulo);      // Saída: null
console.log(valorIndefinido); // Saída: undefined


Claro, aqui está o roteiro completo em formato Markdown, incluindo todos os conceitos e o programa da calculadora atualizado:

markdown
Copy code
# Roteiro de Ensino de JavaScript

## Seção 1: Introdução ao JavaScript

**Conceito:** JavaScript na web e Tipagem Fraca

**Exemplo:** Variáveis em JavaScript podem ter tipos variados:
```javascript
let x = 10;       // x é um número
x = "Hello";      // x agora é uma string
x = true;         // x agora é um booleano
Seção 2: Variáveis com var, let e const
Conceito: Diferenças entre var, let, e const

var: Escopo de função ou global, permite reatribuição.
let: Escopo de bloco, permite reatribuição.
const: Escopo de bloco, não permite reatribuição (valor constante).
Exemplo:

javascript
Copy code
let a = 10;
let b = 20;
const c = 30;

a = 5;   // Isso é permitido com var
b = 15;  // Isso é permitido com let
// c = 25;  // Isso gerará um erro, pois c é constante
Seção 3: Tipos de Dados em JavaScript
Number
Conceito: O tipo Number representa valores numéricos, inteiros ou de ponto flutuante.

Exemplo: Declarando e usando números em JavaScript.

javascript
Copy code
let idade = 30;
let preco = 19.99;
Math
Conceito: O objeto Math fornece funções matemáticas para realizar cálculos complexos.

Exemplo: Usando o objeto Math para calcular a raiz quadrada.

javascript
Copy code
let numero = 16;
let raizQuadrada = Math.sqrt(numero);
console.log(raizQuadrada); // Saída: 4
String
Conceito: O tipo String representa sequências de caracteres.

Exemplo: Declarando e manipulando strings.

javascript
Copy code
let saudacao = "Olá, mundo!";
let comprimento = saudacao.length; // Retorna 12
Template String
Conceito: Template strings são strings que permitem interpolação de variáveis e quebras de linha.

Exemplo: Usando template strings para criar mensagens formatadas.

javascript
Copy code
let nome = "Alice";
let mensagem = `Bem-vindo(a), ${nome}!`;
console.log(mensagem); // Saída: Bem-vindo(a), Alice!
Boolean
Conceito: O tipo Boolean representa valores lógicos verdadeiro (true) ou falso (false).

Exemplo: Usando booleanos em expressões lógicas.

javascript

let temPermissao = true;
let estaLogado = false;
let resultado = temPermissao && estaLogado; // Retorna false
Array
Conceito: Um array é uma coleção ordenada de valores, que podem ser de diferentes tipos.

Exemplo: Declarando e acessando elementos de um array.

javascript

let frutas = ["maçã", "banana", "laranja"];
console.log(frutas[0]); // Saída: maçã
Object
Conceito: Um objeto é uma coleção de pares chave-valor que permite armazenar e acessar dados de maneira estruturada.

Exemplo: Declarando e acessando propriedades de um objeto.

javascript

let pessoa = {
    nome: "João",
    idade: 25,
    cidade: "São Paulo"
};

console.log(pessoa.nome); // Saída: João

Null e Undefined

Conceito: null representa a ausência intencional de qualquer valor ou objeto. undefined é usado quando uma variável foi declarada, mas ainda não foi atribuída um valor.

Exemplo: Demonstrando o uso de null e undefined.

javascript

let valorNulo = null;
let valorIndefinido;
console.log(valorNulo);      // Saída: null
console.log(valorIndefinido); // Saída: undefined
Seção 4: Programa da Calculadora JavaScript
HTML

<!DOCTYPE html>
<html>
<head>
    <title>Calculadora JavaScript</title>
</head>
<body>
    <h1>Calculadora JavaScript</h1>
    <label for="numeros">Insira os números (separados por vírgulas):</label>
    <input type="text" id="numeros">
    <select id="operacao">
        <option value="soma">Soma</option>
        <option value="subtracao">Subtração</option>
        <option value="multiplicacao">Multiplicação</option>
        <option value="divisao">Divisão</option>
    </select>
    <button onclick="calcular()">Calcular</button>
    <p id="resultado"></p>

    <script>
        function calcular() {
            const numerosStr = document.getElementById("numeros").value;
            const numeros = numerosStr.split(",").map(parseFloat);
            const operacao = document.getElementById("operacao").value;
            let resultado;

            switch (operacao) {
                case "soma":
                    resultado = numeros.reduce((acc, num) => acc + num, 0);
                    break;
                case "subtracao":
                    resultado = numeros.reduce((acc, num) => acc - num);
                    break;
                case "multiplicacao":
                    resultado = numeros.reduce((acc, num) => acc * num, 1);
                    break;
                case "divisao":
                    if (numeros.includes(0)) {
                        resultado = "Não é possível dividir por zero.";
                    } else {
                        resultado = numeros.reduce((acc, num) => acc / num);
                    }
                    break;
                default:
                    resultado = "Operação inválida.";
            }

            document.getElementById("resultado").textContent = `Resultado: ${resultado}`;
        }
    </script>
</body>
</html>