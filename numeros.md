# Números

A linguagem trabalha com os seguintes valores numéricos:

* Números inteiros;
* Números fracionários;
* Números mistos;
* Números hexadecimais;

## Números inteiros

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

`Uma fração é uma estrutura com`

&#x20; `Um numerador e`

&#x20; `Um denominador.`

## Números mistos

`Um numeral misto é uma estrutura com`&#x20;

&#x20; `Um número inteiro e`&#x20;

&#x20; `Uma proporção e`&#x20;

&#x20; `Uma fração`` `_`sob`_` ``a proporção.`
