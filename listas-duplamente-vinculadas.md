# Listas duplamente vinculadas

Uma lista encadeada ou lista ligada é uma [estrutura de dados](https://pt.wikipedia.org/wiki/Estrutura\_de\_dados) linear e dinâmica. Ela é composta por várias elementos que estão interligados através de [ponteiros](https://pt.wikipedia.org/wiki/Ponteiro\_\(programa%C3%A7%C3%A3o\)), ou seja, cada elemento da lista possui um ponteiro que aponta para o [endereço de memória](https://pt.wikipedia.org/wiki/Endere%C3%A7o\_\(mem%C3%B3ria\)) da próxima célula. Desse modo, os elementos da lista não precisam estar em posições contíguas da memória. Isso faz com que a estrutura se torne dinâmica, pois a qualquer momento, é possível incluir uma novo elemento na lista, bastando ajustar os ponteiros das células já existentes, de modo que a nova célula seja inserida na estrutura com êxito, na posição desejada pelo programador.

Você pode declarar listas usando a seguinte sintaxe:

```
A Bíblia é uma lista com uns versos.
Um verso é uma lista com uma string.
```

O compilador irá, internamente, converter as declarações acima, nas estruturas abaixo:

```
Um verso é um ponteiro para uma estrutura de versos.

Uma estrutura de versos é uma estrutura com
  Um próximo verso,
  Um verso anterior e 
  Uma string.
  
Uns versos são uma lista com
  Um primeiro verso e
  Um último verso.
```

Na Biblioteca padrão existem diversas rotinas para trabalhar com listas.&#x20;

Exemplos:

```
ACRESCENTE uma lista para umas listas. 
ACRESCENTE umas listas para umas outras listas. 
INSIRA uma lista em umas listas APÓS uma outra lista. 
INSIRA umas listas em umas outras listas APÓS uma lista.
INSIRA uma lista em umas listas ANTES DE uma outra lista. 
INSIRA umas listas em umas outras listas ANTES DE uma lista. 
MOVA uma lista de umas listas para outras listas. 
MOVA umas listas para umas outras listas. 
ANTEPONHA uma lista para umas listas. 
ANTEPONHA umas listas para umas outras listas. 
REVERTA umas listas.
REMOVA uma lista desde umas listas. 
```

Exemplo de utilização:

&#x20;<mark style="color:blue;">`Acrescente o verso para os versos.`</mark>

<mark style="color:blue;">`Insira o verso após os outros versos.`</mark>

&#x20;<mark style="color:blue;">`Remova o verso desde os versos.`</mark>

A Biblioteca padrão também contém rotinas para <mark style="color:blue;">`"Atribuir a quantidade de elementos de uma lista para uma contagem."`</mark>

_<mark style="color:red;">As listas são alocadas dinamicamente então é necessário efetuar a alocação e desalocação de memória das listas manualmente, de forma explícita.</mark>_

Exemplos de alocação:

<mark style="color:blue;">`Crie a Bíblia.`</mark>

<mark style="color:blue;">`Aloque memória para a Bíblia.`</mark>

Exemplos de desalocação:

<mark style="color:red;">`Destrua a Bíblia.`</mark>

<mark style="color:red;">`Desaloque a Bíblia.`</mark>

Perceba que ao destruir uma lista, todos os seus elementos são destruídos juntamente com ela.

Para evitar este comportamento, utilize a palavra-chave "**(referência)"** após o nome do elemento.

Exemplos:

```
Um campo de estrutura é uma estrutura com
  Um sinalizador de redirecionamento,
  Um campo (referência),
  Uma rotina de função (referência),
  Um sinalizador de empilhamento.

Uma unidade semântica é uma lista com
  Uma string,
  Um tipo (referência),
  Uma variável (referência),
  Um tipo atual (referência),
  Um subtexto atual.
```
