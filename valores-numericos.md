# Valores numéricos

A linguagem trabalha com os seguintes valores numéricos:

* Números inteiros;
* Números fracionários;
* Números mistos;
* Números hexadecimais;

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

&#x20;<mark style="color:blue;">`\ Devido à extremidade (ordenação) dos processadores x86`</mark>

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

Os valroes hexadecimais são prefixados com o caractere <mark style="color:blue;">`$`</mark>.

Exemplos:

<mark style="color:blue;">`$DEADBEEF`</mark>

<mark style="color:blue;">`$0D0A`</mark>

## Ponteiros

Um ponteiro é uma estrutura com 4 bytes, funcionando de forma similar a um número, no sentido que é possível&#x20;



## Valores booleanos

Existem 2 valroes booleanos:

<mark style="color:blue;">`sim`</mark> (valor 1)

e&#x20;

<mark style="color:blue;">`não`</mark> (valor 0)
