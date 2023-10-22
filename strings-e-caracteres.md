# Strings e caracteres

## Caracteres

O compilador trabalha com os caracteres constantes na [code page](https://en.wikipedia.org/wiki/Code\_page) [Windows 1252](https://en.wikipedia.org/wiki/Windows-1252) ([ISO-8859-1](https://pt.wikipedia.org/wiki/ISO/IEC\_8859-1)).&#x20;

A lista é composta dos 256 caracteres listados abaixo, incluindo [caracteres de  controle](https://pt.wikipedia.org/wiki/Caractere\_de\_controle).

``␀ ␁ ␂ ␃ ␄ ␅ ␆ ␇ ␈ ␉ ␊ ␋ ␌ ␍ ␎ ␏ ␐ ␑ ␒ ␓ ␔ ␕ ␖ ␗ ␘ ␙ ␚ ␛ ␜ ␝ ␞ ␟ ! " # $ % & ' ( ) * + , - . / 0 1 2 3 4 5 6 7 8 9 : ; < = > ? @ A B C D E F G H I J K L M N O P Q R S T U V W X Y Z [ \ ] ^ _ ` a b c d e f g h i j k l m n o p q r s t u v w x y z { | } ~ ? € ‚ ƒ „ … † ‡ ˆ ‰ Š ‹ Œ Ž ‘ ’ “ ” • – — ˜ ™ š › œ ž Ÿ ¡ ¢ £ ¤ ¥ ¦ § ¨ © ª « ¬ ® ¯ ° ± ² ³ ´ µ ¶ · ¸ ¹ º » ¼ ½ ¾ ¿ À Á Â Ã Ä Å Æ Ç È É Ê Ë Ì Í Î Ï Ð Ñ Ò Ó Ô Õ Ö × Ø Ù Ú Û Ü Ý Þ ß à á â ã ä å æ ç è é ê ë ì í î ï ð ñ ò ó ô õ ö ÷ ø ù ú û ü ý þ ÿ``



Abaixo temos a implementação do tipo caractere:

`Um caractere é um byte.` <mark style="color:blue;">\ 1 byte = 8 bits</mark>

Um byte são 8 bits sequenciais de dados binários. São  números sem sinal, com valores variando de 0 a 255.



## Strings

Strings são delimitadas com aspas duplas.

_Exemplo:_

`O servidor SMTP padrão é uma string igual a`<mark style="color:blue;">`"localhost"`</mark>`.`

`Atribua`<mark style="color:blue;">`"José"`</mark>`ao nome desta pessoa.`

`Se o nome desta pessoa for`<mark style="color:blue;">`"João"`</mark>`, retorne.`



Utilizamos aspas duplas como [caractere de escape](https://pt.wikipedia.org/wiki/Caractere\_de\_escape).

_Exemplo:_

`Atribua`` `<mark style="color:blue;">`"Erro. A palavra chave ""`</mark><mark style="color:green;">`Itere`</mark><mark style="color:blue;">`"" não foi localizada."`</mark>` ``à mensagem de erro.`



No código abaixo temos a implementação do tipo string:

> Uma string é uma <mark style="color:blue;">estrutura</mark> com&#x20;
>
> &#x20; Um caractere inicial e&#x20;
>
> &#x20; Um caractere final.

_Sendo que_

> Um caractere inicial é um ponteiro <mark style="color:blue;">\[que aponta]</mark> para um byte.&#x20;
>
> Um caractere final é um ponteiro <mark style="color:blue;">\[que aponta]</mark> para um byte.



Perceba que o compilador armazena "strings" em duas partes:&#x20;

1. Uma <mark style="color:blue;">`estrutura`</mark> com um par de _ponteiros de bytes_ denominados<mark style="color:blue;">`caractere inicial`</mark> e <mark style="color:blue;">`caractere final`</mark>, e
2. Um array dinâmico que contém os bytes reais da string, de forma similar à imagem abaixo:

<figure><img src=".gitbook/assets/image (3).png" alt="Figura 1 - Representação de um array com os dados da string, contendo o caractere o endereço na memória."><figcaption><p>Figura 1 - Representação de um array com os dados da string, contendo o caractere o endereço na memória.</p></figcaption></figure>

Observação: os números no diagrama acima, são endereços fictícios.

Uma string é considerada <mark style="color:blue;">`em branco`</mark> se o caractere inicial for inexistente (ou seja, nenhuma memória foi alocada ainda) ou se o endereço do <mark style="color:blue;">`caractere final`</mark> for menor do que o endereço do <mark style="color:blue;">`caractere inicial`</mark> (o que permite ao compilador realizar pré-alocação de memória).

As strings são alocadas dinamicamente e podem ter qualquer comprimento - mas a memória de strings é gerenciada inteiramente (e de forma muito eficiente) pelo compilador, quase como se fossem alocadas estaticamente. Em outras palavras, você não precisa se se preocupar com elas, pois o compilador gerencia a alocação e desalocação de forma automática.&#x20;

## Manipulando strings

Na Biblioteca padrão existem diversas rotinas para manipulação de strings.&#x20;

Exemplos:

`ATRIBUA variável PARA uma string.`&#x20;

`ACRESCENTE algo PARA uma string.`&#x20;

`INSIRA algo EM uma STRING antes de um caractere.`&#x20;

`REMOVA O CARACTERE INICIAL DE uma string.`&#x20;

`REMOVA O CARACTERE FINAL DE uma string.`&#x20;

`PREENCHA uma string COM um CARACTERE USANDO uma quantidade.`&#x20;

`REMOVA OS CARACTERES INICIAIS DE uma string USANDO uma quantidade.`&#x20;

`REMOVA OS CARACTERES FINAIS DE uma string COM UMA quantidade.`&#x20;

`REMOVE OS CARACTERES DE uma string DADA uma substring.`&#x20;



Você também pode alterar uma string para deixar o texto em **LETRAS MAIÚSCULAS** ou em  **letras minúsculas**. (Ou alterar apenas a primeira letra para letras maiúsculas).

E você pode, é claro, obter o comprimento de uma string, em bytes.&#x20;

Exemplo:

`Atribua "João" para uma string.`

`Atribua o comprimento desta string para um número.`



Além disso, você pode concatenar strings com strings — e outros tipos de dados — usando o operador <mark style="color:blue;">`junto com`</mark> ou <mark style="color:blue;">`seguido de`</mark>.

Exemplo:

`Atribua o nome`` `<mark style="color:blue;">`junto com`</mark>` ``o sobrenome para uma string.`

`Escreva "Erro #"`` `<mark style="color:blue;">`junto com`</mark>` ``o número do erro`` `<mark style="color:blue;">`seguido de`</mark>` ``"." no console.`

## Subtextos

Um "subtexto" faz parte de uma string. Os subtextos são implementadas como uma estrutura igual a uma string — um par de ponteiros de bytes chamados caractere inicial e caractere final — o que torna o subtexto compatível com o tipo string.

O comando:

`Lance um subtexto em uma string.`&#x20;

Faz com que o `caractere inicial` e o `caractere final` do subtexto englobem toda a string.&#x20;

Dessa forma você pode percorrer através dos caracteres da string, indo para frente ou para trás. Para iso basta incrementar o valor do endereço do caractere inicial ou reduzir o valor do endereço do caractere final do subtexto.

Você também pode usar o comando:&#x20;

`POSICIONE uma substring em uma string.`&#x20;

O comando acima define apenas o caractere inicial do subtexto, deixando o valor do caractere final inicialmente em branco, porém pronto para ser alterado. Ao definir e incrementar o valor do caractere final, você pode ir criando a substring um byte de cada vez.

As substrings são utilizadas principalmente de forma conjunta com "percorredores".

## Trabalhando com Percorredores

Parsing é o ato de percorrer um bloco de texto, um pedaço de cada vez, onde um pedaço pode ser tão pequeno quanto uma letra ou tão grande quanto o bloco inteiro.&#x20;

Vamos usar a string abaixo como nosso bloco de texto de exemplo:&#x20;

**"The quick brown fox jumps over the lazy dog"**&#x20;

Digamos que queremos extrair cada uma das palavras individuais da string acima.&#x20;

As ferramentas que usaremos serão&#x20;

1. o subtexto, e
2. o percorredor

**Um percorredor é definido da seguinte forma:**

> Um percorredor é uma estrutura com&#x20;
>
> &#x20; Uma cópia da string original,
>
> &#x20; Um segmento final,&#x20;
>
>
>
> Uma cópia da string original é um subtexto.&#x20;
>
> Um segmento inicial é um subtexto.&#x20;
>
> Um segmento final é um subtexto.



Quando você "lançar" um subtexto na string acima, o compilador irá definir o caractere inicial do subtexto como **"T"** (da palavra **The**) e o caractere inicial como **"g"** (da palavra **dog**).

Ao usar o comando:

`"Lance um percorredor sobre o subtexto"`

Os membros do percorredor ficarão assim:

* cópia da string original = "**The quick brown fox jumps over the lazy dog"**
* segmento inicial = ""
* segmento final = "**The quick brown fox jumps over the lazy dog"**

A partir daí podemos invocar a rotina

`Mova o percorredor (strings com aspas).`

Neste momento, os membros do percorredor ficarão assim:

* cópia da string original = "**The quick brown fox jumps over the lazy dog"**
* segmento inicial = "**The**"
* segmento final = "**quick brown fox jumps over the lazy dog"**

Se reperirmos o comando, os membros do percorredor ficarão assim:

* cópia da string original = "**The quick brown fox jumps over the lazy dog"**
* segmento inicial = "**quick**"
* segmento final = "**brown fox jumps over the lazy dog"**

Perceba que o "**The"** foi "removido" do segmento inicial.

