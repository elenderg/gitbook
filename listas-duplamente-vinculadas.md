# Listas duplamente vinculadas

Uma lista encadeada ou lista ligada é uma [estrutura de dados](https://pt.wikipedia.org/wiki/Estrutura\_de\_dados) linear e dinâmica. Ela é composta por várias elementos que estão interligados através de [ponteiros](https://pt.wikipedia.org/wiki/Ponteiro\_\(programa%C3%A7%C3%A3o\)), ou seja, cada elemento da lista possui um ponteiro que aponta para o [endereço de memória](https://pt.wikipedia.org/wiki/Endere%C3%A7o\_\(mem%C3%B3ria\)) da próxima célula. Desse modo, os elementos da lista não precisam estar em posições contíguas da memória. Isso faz com que a estrutura se torne dinâmica, pois a qualquer momento, é possível incluir uma novo elemento na lista, bastando ajustar os ponteiros das células já existentes, de modo que a nova célula seja inserida na estrutura com êxito, na posição desejada pelo programador.

Você pode declarar listas usando a seguinte sintaxe:



`A Bíblia é uma`` `<mark style="color:blue;">`lista com`</mark>` ``uns versos.`

`Um verso é uma`` `<mark style="color:blue;">`lista com`</mark>` ``uma string.`



O compilador irá, internamente, converter as declarações acima, nas estruturas abaixo:

`Um verso é um`` `<mark style="color:blue;">`ponteiro para`</mark>` ``uma estrutura de versos.`

`Uma estrutura de versos é uma`` `<mark style="color:blue;">`estrutura`</mark>` ``com`

&#x20; `Um`<mark style="color:green;">`próximo`</mark>`verso,`

&#x20; `Um verso`<mark style="color:green;">`anterior`</mark>`e`&#x20;

&#x20; `Uma string.`

`Uns versos são uma lista com`

&#x20; `Um`<mark style="color:green;">`primeiro`</mark>`verso e`

&#x20; `Um`<mark style="color:green;">`último`</mark>`verso.`



Na Biblioteca padrão existem diversas rotinas para trabalhar com listas.&#x20;

Exemplos:



`ACRESCENTE uma lista para umas listas.`&#x20;

`ACRESCENTE umas listas para umas outras listas.`&#x20;

Exemplo:  `Acrescente o verso para os versos.`



`INSIRA uma lista em umas listas APÓS uma outra lista.`&#x20;

`INSIRA umas listas em umas outras listas APÓS  uma lista.`&#x20;

Exemplo:  `Insira o verso após os outros versos.`



`INSIRA uma lista em umas listas ANTES DE uma outra lista.`&#x20;

`INSIRA umas listas em umas outras listas ANTES DE uma lista.`&#x20;

`MOVA uma lista de umas listas para outras listas.`&#x20;

`MOVA umas listas para umas outras listas.`&#x20;

`ANTEPONHA uma lista para umas listas.`&#x20;

`ANTEPONHA umas listas para umas outras listas.`&#x20;



`REMOVA uma lista desde umas listas.`&#x20;

Exemplo:  `Remova o verso desde os versos.`



`REVERTA umas listas.`

A Biblioteca padrão também contém rotinas para "Atribuir a quantidade de elementos de uma lista para uma contagem."



_<mark style="color:red;">As listas são alocadas dinamincamente então é necessário efetuar a alocação e desalocação de memória das listas manualmente, de forma explícita.</mark>_

