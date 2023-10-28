# Rotinas, Parâmetros e Funções

A sintaxe básica para declaração de uma rotina é a seguinte:

<mark style="color:blue;">`Rotina para que se`</mark><mark style="color:green;">`<nome da rotina>`</mark><mark style="color:red;">`:`</mark>

O nome da rotina começa após o **"se"**.&#x20;

Parâmetros são indicados pelos artigos indefinidos:&#x20;

* **um**
* **uns**
* **uma**
* **umas**

Exemplos:



<mark style="color:blue;">`Rotina para que se`</mark> <mark style="color:green;">`adicione`</mark> <mark style="color:purple;">`uma`</mark>` ``cor`` `<mark style="color:red;">`e`</mark> <mark style="color:purple;">`um`</mark>` ``rótulo`` `<mark style="color:red;">`para`</mark>` `<mark style="color:purple;">`um`</mark>` ``menu:`

**Nome da rotina:** adicione

**Parâmetros:** cor, rótulo, menu

**Preposições e conjunções:** e, para.



<mark style="color:blue;">`Rotina para que se`</mark> <mark style="color:green;">`crie`</mark>` `<mark style="color:purple;">`uma`</mark>` ``imagem`` `<mark style="color:red;">`usando`</mark>` `<mark style="color:purple;">`uma`</mark>` ``URL:`

**Nome da rotina:** crie

**Parâmetros:** imagem, URL

**Preposições e conjunções:** usando

As preposições e conjunções embora não façam parte do nome da rotina, devem ser utilizadas de forma similar ao declarado. A 1ª rotina acima pode ser chamada de forma similar ao exemplo abaixo:

```
Adicione a cor preta e "Abrir" para o menu.
Adicione a cor vermelha e "Fechar" ao menu.
```

A 2ª rotina, por exemplo poderia ser chamada das seguintes formas:

```
Crie a imagem usando a URL.
Crie a imagem dada a URL.
Crie a imagem com a URL.
Crie a imagem desde a URL.
```

{% hint style="info" %}
Perceba que a linguagem suporta:

**Contrações em geral\***

* à -> para a
* ao -> para o
* deste -> de este
* destes -> de estes
* desta -> de estas
* destas -> de estas
* desta -> de esta
* na -> em a
* nas -> em as
* no -> em o
* nos -> em os
* num -> em um
* nuns -> em uns
* numa -> em uma
* numas -> em umas
* pelo -> por o
* pelos -> por os
* pela -> por a
* pelas -> por as

**Sinônimos** (para as preposições).&#x20;

* com / contendo / dado / desde / usando
* em / para / por
{% endhint %}

Para um melhor entendimento da linguagem iremos converter a função Javascript abaixo para Português Puro:

{% code lineNumbers="true" %}
```javascript
function FazAlgumaCoisa(numero) {
  if(number < 0){
    return;
    }
  let contador = numero *2;
  while (true) {
    contador ++;
    if (contador >= 10) {
      break;
    }
  }
}
```
{% endcode %}

**Dados da função**

**Nome:** FazAlgumaCoisa.

**Parâmetros:** numero.

**Variáveis locais:** contador.

**Número de linhas:** **12**

_<mark style="color:blue;">A rotina acima ficaria assim:</mark>_

> **Para que se** _faça alguma coisa_ com <mark style="color:purple;">**um**</mark> número:&#x20;
>
> &#x20; Se <mark style="color:purple;">**o**</mark> número for menor do que 0, _<mark style="color:blue;">**retorne**</mark>_.&#x20;
>
> &#x20; Atribua <mark style="color:purple;">**o**</mark> número vezes 2 para <mark style="color:red;">**um**</mark> contador.&#x20;
>
> &#x20; _<mark style="color:blue;">**Itere**</mark>_.&#x20;
>
> &#x20;   Adicione 1 para <mark style="color:red;">**o**</mark> contador.&#x20;
>
> &#x20;   Se <mark style="color:red;">**o**</mark> contador for maior do que 10, _<mark style="color:blue;">**pare**</mark>_.&#x20;
>
> &#x20; _<mark style="color:blue;">**Reitere**</mark>_.

**Dados da rotina**

**Nome:** Faça alguma coisa

**Parâmetros:** número

**Variáveis locais:** contador.

**Número de linhas: 7**

Perceba que ao invés da keyword _**function**_ nós utilizamos _**para que se** (o termo "Rotina" é opcional)._

Perceba que o parâmetros <mark style="color:purple;">**"número"**</mark> bem como a variável local <mark style="color:red;">**"contador"**</mark> foram referenciados com um artigo definido após serem introduzidas no código pela 1ª vez com um artigo indefinido.

## Funções de retorno booleano

A linguagem trabalha com o conceito de "funções deliberativas".

Para criar uma função decisória a sintaxe utilize a seguinte sintaxe:

> **Para que se determine se** <mark style="color:purple;">**um**</mark> número _<mark style="color:red;">**é**</mark>_ negativo:&#x20;
>
> &#x20; Se <mark style="color:purple;">**o**</mark> número for menor do que 0, <mark style="color:green;">diga sim.</mark>&#x20;
>
> &#x20; <mark style="color:blue;">\ Caso contrário</mark>
>
> &#x20; <mark style="color:red;">Diga não.</mark>

<mark style="color:green;">"Diga sim"</mark> equivale a um <mark style="color:green;">"return true"</mark> e <mark style="color:red;">"Diga não"</mark> é o equivalente de <mark style="color:red;">"return false"</mark>.

As funções deliberativas costumam ser utilizadas dentro de declarações condicionais.

Por exemplo:

_**`Se o número`****` `**<mark style="color:red;">**`for`**</mark>**` `****`negativo, retorne.`**_

{% hint style="info" %}
Os verbos ser/estar (e suas respectivas conjugações) são tratados como sinônimos pelo compilador.
{% endhint %}

## Regras gerais para nomes de rotinas e funções

* O nome da rotina começa após o _"para que se"_ (ou após o _"para que se determine se"_ no caso de funções deliberativas).
* Artigos indefinidos indicam um novo parâmetro. Exemplos:
  * _um número,_
  * _uns vértices,_
  * _uma string,_
  * _umas formas_
* Parênteses podem ser utilizados para "escapar" strings, parâmetros ou indicar rotinas de um mesmo grupo. Exemplo:
  * _Rotina para que se execute um evento (clique - botão direito):_&#x20;
  * _Rotina para que se execute um evento (clique - botão esquerdo):_&#x20;
  * _Rotina para que se execute um evento (clique duplo):_&#x20;
  * _Rotina para que se execute um evento (atualização de tela):_&#x20;
* Preposições e artigos definidos são permitidos nos nomes das rotinas (porém não exercem nenhuma função especial além de tornar o nome da função mais inteligível). Exemplos:
  * _Rotina para que se execute **o** programa:_
  * _Rotina para que se ajuste **a** caixa de diálogo:_
  * _Rotina para que se adicione um botão **para a** caixa de diálogo **usando** uma string:_

{% hint style="info" %}
Perceba nas rotinas logo acima que os artigos definidos **não** indicam um parâmetro.&#x20;
{% endhint %}
