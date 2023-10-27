# Rotinas, Parâmetros e Funções

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



A rotina acima ficaria assim:

{% code lineNumbers="true" %}
```textile
Rotina para que se faça alguma coisa com um número:
  Se o número for menor do que 0, retorne.
  Atribua o número vezes 2 para um contador.
  Itere.
    Adicione 1 para o contador.
    Se o contador for maior do que 10, pare.
  Reitere.
```
{% endcode %}

**Dados da rotina**

**Nome:** Faça alguma coisa

**Parâmetros:** número

**Variáveis locais:** contador.

**Número de linhas: 7**

## Funções de retorno booleano

Para criar uma função booleana a sintaxe utilize a seguinte sintaxe:

> **Para que se determine se** um número _é_ negativo:&#x20;
>
> &#x20; Se o número for menor do que 0, <mark style="color:green;">diga sim.</mark>&#x20;
>
> &#x20; <mark style="color:blue;">\ Caso contrário</mark>
>
> &#x20; <mark style="color:red;">Diga não.</mark>

<mark style="color:green;">"Diga sim"</mark> equivale a um <mark style="color:green;">"return true"</mark> e <mark style="color:red;">"Diga não"</mark> é o equivalente de <mark style="color:red;">"return false"</mark>.

Perceba que ao invés da keyword _**function**_ nós utilizamos _**para que se** (o termo "Rotina" é opcional)._

A sinatxe básica é a seguinte:

<mark style="color:blue;">`<para que se>`</mark><mark style="color:green;">`<nome da rotina>`</mark><mark style="color:red;">`:`</mark>

O nome da rotina começa após o 1º **"se"** (em caso de rotinas) ou após **"determine se"** (no caso das funções booleanas).&#x20;

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

