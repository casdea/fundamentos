# Roteiro de Ensino de JavaScript

## Seção 1: Introdução ao JavaScript

**Conceito:** JavaScript na web e Tipagem Fraca

**Exemplo:** Variáveis em JavaScript podem ter tipos variados:

```javascript
var x = 10;       // x é um número
x = "Hello";      // x agora é uma string
x = true;         // x agora é um booleano

Seção 2: Variáveis com var, let e const

Conceito: Diferenças entre var, let, e const

var: Escopo de função ou global, permite reatribuição.
let: Escopo de bloco, permite reatribuição.
const: Escopo de bloco, não permite reatribuição (valor constante).

Exemplo:

var a = 10;
let b = 20;
const c = 30;

a = 5;   // Isso é permitido com var
b = 15;  // Isso é permitido com let
// c = 25;  // Isso gerará um erro, pois c é constante

Seção 3: Atualizando o Projeto da Calculadora

Atualize o projeto da calculadora para usar let e const, e explique como a tipagem fraca funciona ao receber valores do usuário.

HTML:

<!DOCTYPE html>
<html>
<head>
    <title>Calculadora Simples</title>
</head>
<body>
    <h1>Calculadora Simples</h1>
    <input type="number" id="numero1">
    <input type="number" id="numero2">
    <button onclick="somar()">Somar</button>
    <button onclick="subtrair()">Subtrair</button>
    <button onclick="multiplicar()">Multiplicar</button>
    <button onclick="dividir()">Dividir</button>
    <p id="resultado"></p>

    <script>
        // Funções para realizar operações
        function somar() {
            const num1 = parseFloat(document.getElementById("numero1").value);
            const num2 = parseFloat(document.getElementById("numero2").value);
            const resultado = num1 + num2;
            document.getElementById("resultado").textContent = "Resultado: " + resultado;
        }

        function subtrair() {
            let num1 = parseFloat(document.getElementById("numero1").value);
            let num2 = parseFloat(document.getElementById("numero2").value);
            const resultado = num1 - num2;
            document.getElementById("resultado").textContent = "Resultado: " + resultado;
        }

        function multiplicar() {
            let num1 = parseFloat(document.getElementById("numero1").value);
            let num2 = parseFloat(document.getElementById("numero2").value);
            const resultado = num1 * num2;
            document.getElementById("resultado").textContent = "Resultado: " + resultado;
        }

        function dividir() {
            let num1 = parseFloat(document.getElementById("numero1").value);
            let num2 = parseFloat(document.getElementById("numero2").value);
            if (num2 !== 0) {
                const resultado = num1 / num2;
                document.getElementById("resultado").textContent = "Resultado: " + resultado;
            } else {
                document.getElementById("resultado").textContent = "Não é possível dividir por zero.";
            }
        }
    </script>
</body>
</html>

Seção 4: Tipos de Dados em JavaScript
Number
Conceito: O tipo Number representa valores numéricos, inteiros ou de ponto flutuante.

Exemplo: Declarando e usando números em JavaScript.

let idade = 30;
let preco = 19.99;

Math

Conceito: O objeto Math fornece funções matemáticas para realizar cálculos complexos.

Exemplo: Usando o objeto Math para calcular a raiz quadrada.

javascript

let numero = 16;
let raizQuadrada = Math.sqrt(numero);
console.log(raizQuadrada); // Saída: 4

String

Conceito: O tipo String representa sequências de caracteres.

Exemplo: Declarando e manipulando strings.

