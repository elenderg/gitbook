# Estruturas e Uniões de dados

Uma [estrutura](https://en.wikipedia.org/wiki/Record\_\(computer\_science\)) é um tipo de dado composto, cujo interior abriga uma quantidade qualquer de variáveis denominadas "campos" ou "membros".&#x20;

Exemplo:&#x20;

```
Uma string é uma estrutura com 
  Um caractere inicial e 
  Um caractere final.
```

Uma estrutura vazia ocupa 0 bits na memória, mas você pode definir estruturas de qualquer comprimento adicionando "campos" ou "membros" ao protótipo da estrutura. Esses campos podem ser de qualquer tipo.

O tamanho da estrutura é, em via de regra, igual à soma do tamanho de seus campos.

Perceba que a estrutura acima contém 02 membros: o **caractere inicial** e o **caractere final**. isto só é possível por causa que estes tipos já haviam sido declarados previamente (caso contrário o compilador emitiria uma mensagem de erro informando que o tipo de dado declarado não foi reconhecido).&#x20;

Não é necessário declarar um novo tipo de dado para cada membro de uma estrutura. Se o tipo de dado for utilizado apenas dentro do contexto da estrutura, você pode utilizar a palavra-chave **"denominado"** (e suas respectivas flexões em gênero e número).

A sintaxe geral é:

`<artigo indefinido> <tipo>`` `<mark style="color:blue;">`denominado`</mark>` ``<nome>`

Exemplo:

```
Um DEVMODE é uma estrutura com
\ Contém informações sobre a inicialização de uma impressora ou monitor de vídeo.
  32 bytes denominados dmDeviceName,
  Uma word denominada dmSpecVersion,
  Uma word denominada dmDriverVersion,
  Uma word denominada dmSize,
  Uma word denominada dmDriverExtra,
  Um número denominado dmFields,
  Uma word denominada dmOrientation,
  Uma word denominada dmPaperSize,
  Uma word denominada dmPaperLength,
  Uma word denominada dmPaperWidth,
  Uma word denominada dmScale,
  Uma word denominada dmCopies,
  Uma word denominada dmDefaultSource,
  Uma word denominada dmPrintQuality,
  Uma word denominada dmColor,
  Uma word denominada dmDuplex,
  Uma word denominada dmYResolution,
  Uma word denominada dmTTOption,
  Uma word denominada dmCollate,
  32 bytes denominados dmFormName,
  Uma word denominada dmLogPixels,
  Um número denominado dmBitsPerPel,
  Um número denominado dmPelsWidth,
  Um número denominado dmPelsHeight,
  Um número denominado dmDisplayFlags,
  Um número denominado dmDisplayFrequency,
  Um número denominado dmICMMethod,
  Um número denominado dmICMIntent,
  Um número denominado dmMediaType,
  Um número denominado dmDitherType,
  Um número denominado dmReserved1,
  Um número denominado dmReserved2.
```

## Uniões de dados

Uma união é um valor que pode ter várias representações ou formatos dentro da mesma posição na memória.

É possível criar uma "[união](https://en.wikipedia.org/wiki/Union\_type)[ de dados](https://en.wikipedia.org/wiki/Union\_type)" utilizando a palavra-chave <mark style="color:red;">**sob**</mark>.

Exemplo:

```
Um número é uma estrutura com
  Um primeiro byte,
  Um segundo byte,
  Um terceiro byte,
  Um quarto byte,
  Uma word de ordem inferior sob o primeiro byte,
  Uma word de ordem superior sob o terceiro byte.
  
Uma word é uma estrutura com
  Um byte inicial e 
  Um byte final.
```

A estrutura <mark style="color:blue;">`número`</mark>, será armazenada da seguinte forma:\


<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Conforme a implementação dada acima, cada <mark style="color:blue;">`word`</mark> será armazenada da seguinte forma:

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

