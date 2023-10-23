# Valores numéricos

A linguagem trabalha com os seguintes valores numéricos:

* [Números inteiros;](valores-numericos.md#numeros-inteiros)
* [Números fracionários;](valores-numericos.md#numeros-fracionarios)
* [Números mistos;](valores-numericos.md#numeros-mistos)
* [Valores hexadecimais;](valores-numericos.md#valores-hexadecimais)
* [Ponteiros;](valores-numericos.md#ponteiros)
* [Valores booleanos.](valores-numericos.md#valores-booleanos)

## [Words](https://pt.wikipedia.org/wiki/Palavra\_\(ci%C3%AAncia\_da\_computa%C3%A7%C3%A3o\))

As words têm 16 bits,  sendo números com sinal que vão de -32768 a +32767. Devido às particularidades da arquitetura Windows/Intel x86, os bits em cada byte são armazenados da esquerda para a direita, mas os bytes são armazenados inversamente.

## Números inteiros

Um "número" consiste em dígitos, com um sinal opcional, mas sem espaços ou outros símbolos. Exemplos:&#x20;

`0`

`123`

`-2147483648`

`+2147483647`

A implementação de um número de 32 bits é a seguinte:

`Um número é uma estrutura com`&#x20;

&#x20; `Um primeiro byte,`

&#x20; `Um segundo byte,`

&#x20; `Um terceiro byte,`

&#x20; `Um quarto byte,`` `<mark style="color:blue;">`\ 4 bytes = 32 bits`</mark>&#x20;

&#x20; `Uma word de ordem inferior sob o primeiro byte,`&#x20;

&#x20; `Uma word de ordem superior sob o terceiro byte.`

Os números são armazenados de trás para frente devido à extremidade (ordenação) dos processadores x86.



`O menor número é -2147483648.`` `<mark style="color:blue;">`\ número de 4 bytes/32 bits`</mark>

`O maior número é 2147483647.`

## Números fracionários

Uma fração é um número seguido de uma barra e um número sem sinal.&#x20;

Exemplos:&#x20;

`335/113`

`25946/9545`

`-19601/13860`

A implementação de uma fração é a seguinte:

`Uma fração é uma estrutura com`

&#x20; `Um numerador e`

&#x20; `Um denominador.`

## Números mistos

Um número misto é composto de um número, um traço e uma fração sem sinal. Exemplos:

`1-1/2`

`-2-2/3`

`3-3/4`

Abaixo temos a implementação de números mistos:

`Um numeral misto é uma estrutura com`&#x20;

&#x20; `Um número inteiro e`&#x20;

&#x20; `Uma proporção e`&#x20;

&#x20; `Uma fração`` `_`sob`_` ``a proporção.`

## Valores Hexadecimais

Os valores hexadecimais são prefixados com o caractere <mark style="color:blue;">`$`</mark>.

Exemplos:

<mark style="color:blue;">`$DEADBEEF`</mark>

<mark style="color:blue;">`$0D0A`</mark>

## Ponteiros

Um ponteiro é uma estrutura com 4 bytes, funcionando de forma similar a um número, no sentido que é possível efetuar operações aritméticas comuns (soma, subtração, etc).

Os endereços de memória são armazenados em ponteiros de 32 bits, de trás para frente. Eles têm o mesmo intervalo dos números, mas todos os negativos pertencem ao Windows. _O endereço 0 é inválido e é denominado <mark style="color:blue;">nulo</mark> ou <mark style="color:blue;">inexistente</mark>_. **Você pode anular um ponteiro para torná-lo nulo.**

## Valores booleanos

Existem 2 valores booleanos:

<mark style="color:blue;">`sim`</mark> (valor 1)  e  <mark style="color:blue;">`não`</mark> (valor 0).

Eles têm 32 bits, mas apenas o bit mais à direita é usado. Na verdade, é o oitavo da esquerda, mas você pode pensar nele como o mais à direita. O compilador interpreta 0 como “não” e 1 como “sim”.  Você pode desativar um sinalizador para indicar "não" ou ativar um sinalizador para indicar "sim".
