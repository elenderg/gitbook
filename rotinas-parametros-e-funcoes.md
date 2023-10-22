# Rotinas, Parâmetros e Funções

Para um melhor entendimento da linguagem iremos converter a função Javascript abaixo para Português Puro:

{% code lineNumbers="true" %}
```javascript
var soma;
function CalculaSoma(soma, numero) {
    if (numero < 0) {
        return;
    }
    soma = 0;
    let contador = 1;
    while (true) {
        if (contador > numero) {
            break;
        }
        if (contador % 2 !== 0) {
            soma += contador;
        }
        contador++;
    }
}
```
{% endcode %}

**Dados da função**

**Nome:** CalculaSoma.

**Parâmetros:** numero.

**Variáveis locais:** contador.

**Número de linhas:** **17**



A rotina acima ficaria assim:

{% code lineNumbers="true" %}
```textile
Uma soma é um número.

Rotina para que se calcule uma soma usando um número:
  Se o número for menor do que 0, retorne.
  Atribua 0 para a soma.
  Atribua 1 para um contador.
  Itere.
    Se o contador for maior do que o número, pare.
    Se o contador for uniformemente divisível por 2, 
      Adicione o contador à soma.
    Adicione 1 para o contador.
  Reitere.
```
{% endcode %}

**Dados da rotina**

**Nome:** Calcule

**Parâmetros:** soma, número

**Variáveis locais:** contador.

**Número de linhas: 12**



