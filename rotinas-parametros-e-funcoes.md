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

> **Rotina para que se determine se** um número _é_ negativo:&#x20;
>
> &#x20; Se o número for menor do que 0, <mark style="color:green;">diga sim.</mark>&#x20;
>
> &#x20; <mark style="color:blue;">\ Caso contrário</mark>
>
> &#x20; <mark style="color:red;">Diga não.</mark>

<mark style="color:green;">"Diga sim"</mark> equivale a um <mark style="color:green;">"return true"</mark> e <mark style="color:red;">"Diga não"</mark> é o equivalente de <mark style="color:red;">"return false"</mark>.
