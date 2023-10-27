# API Win32 - GdipImageRotateFlip

Observação: para executar este programa salve a imagem abaixo ( ou outra de sua escolha) e ajuste o path onde for necessário.

![](../.gitbook/assets/lobo.png)&#x20;

```
Rotina para que se execute o programa:
  Carregue as bibliotecas padrão do sistema. 
  Limpe a tela usando a cor eigengrau.
  Carregue uma primeira imagem usando "C:\lobo.png".
  Carregue uma segunda imagem usando "C:\lobo.png".
  Carregue uma terceira imagem usando "C:\lobo.png".
  Carregue uma quarta imagem usando "C:\lobo.png".
  Carregue uma quinta imagem usando "C:\lobo.png".
  Carregue uma sexta imagem usando "C:\lobo.png".
  Carregue uma sétima imagem usando "C:\lobo.png".
  Carregue uma oitava imagem usando "C:\lobo.png".
  Mova a primeira imagem usando 50 pixels e 100 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta primeira imagem 
    e o valor da enumeração RotateNoneFlipNone.
  Pinte a primeira imagem.
  Mova a segunda imagem usando 400 pixels e 100 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta segunda imagem 
    e o valor da enumeração Rotate90FlipX.
  Pinte a segunda imagem.
  Mova a terceira imagem usando 800 pixels e 100 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta terceira imagem 
    e o valor da enumeração RotateNoneFlipY.
  Pinte a terceira imagem.
  Mova a quarta imagem usando 1200 pixels e 100 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta quarta imagem 
    e o valor da enumeração RotateNoneFlipXY.
  Pinte a quarta imagem.
  Mova a quinta imagem usando 50 pixels e 500 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta quinta imagem 
    e o valor da enumeração Rotate90FlipY.
  Pinte a quinta imagem.
  Mova a sexta imagem usando 400 pixels e 500 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta sexta imagem 
    e o valor da enumeração Rotate90FlipXY.
  Pinte a sexta imagem.
  Mova a sétima imagem usando 800 pixels e 500 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta sétima imagem 
    e o valor da enumeração RotateNoneFlipNone.
  Pinte a sétima imagem.
  Mova a oitava imagem usando 1200 pixels e 500 pixels.
  Processe "gdiplus.dll" "GdipImageRotateFlip" com 
    o gpBitmap desta oitava imagem 
    e o valor da enumeração RotateNoneFlipX.
  Pinte a oitava imagem.
  Atribua 24 pixels à altura desta fonte padrão.
  Posicione os rótulos.
  Itere.
    Atualize a tela.
    Se a tecla Esc estiver sendo pressionada, pare.
    Se a tecla Enter estiver sendo pressionada, pare.
  Reitere.
  Se a tecla Esc estiver sendo pressionada, 
    Destrua a primeira imagem;
    Destrua a segunda imagem;
    Destrua a terceira imagem;
    Destrua a quarta imagem;
    Destrua a quinta imagem;
    Destrua a sexta imagem;
    Destrua a sétima imagem;
    Destrua a oitava imagem;
    Feche o programa.
  Se a tecla Enter estiver sendo pressionada, 
    Destrua a primeira imagem;
    Destrua a segunda imagem;
    Destrua a terceira imagem;
    Destrua a quarta imagem;
    Destrua a quinta imagem;
    Destrua a sexta imagem;
    Destrua a sétima imagem;
    Destrua a oitava imagem;
    Feche o programa.

Rotina para que se carregue uma imagem usando um endereço completo:
  Leia o endereço completo para a imagem.
  Redimensione a imagem para 300 pixels por 300 pixels.

Um rótulo é uma estrutura com
  Uma caixa e
  Um nome.

Rotina para que se exiba um rótulo:
  Pinte o nome deste rótulo na caixa deste rótulo usando a cor branca.

Rotina para que se posicione os rótulos:
  Posicione o primeiro rótulo.
  Posicione o segundo rótulo.
  Posicione o terceiro rótulo.
  Posicione o quarto rótulo.
  Posicione o quinto rótulo.
  Posicione o sexto rótulo.
  Posicione o sétimo rótulo.
  Posicione o oitavo rótulo.

Rotina para que se posicione o primeiro rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 50 pixels para a coordenada X1 deste primeiro rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 170 pixels para a coordenada Y1 deste primeiro rótulo.
  Atribua o primeiro nome ao nome deste primeiro rótulo.
  Exiba o primeiro rótulo.

Rotina para que se posicione o segundo rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 400 pixels para a coordenada X1 deste segundo rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 170 pixels para a coordenada Y1 deste segundo rótulo.
  Atribua o segundo nome ao nome deste segundo rótulo.
  Exiba o segundo rótulo.

Rotina para que se posicione o terceiro rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 800 pixels para a coordenada X1 deste terceiro rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 170 pixels para a coordenada Y1 deste terceiro rótulo.
  Atribua o terceiro nome ao nome deste terceiro rótulo.
  Exiba o terceiro rótulo.

Rotina para que se posicione o quarto rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 1200 pixels para a coordenada X1 deste quarto rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 170 pixels para a coordenada Y1 deste quarto rótulo.
  Atribua o quarto nome ao nome deste quarto rótulo.
  Exiba o quarto rótulo.

Rotina para que se posicione o quinto rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 50 pixels para a coordenada X1 deste quinto rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 970 pixels para a coordenada Y1 deste quinto rótulo.
  Atribua o quinto nome ao nome deste quinto rótulo.
  Exiba o quinto rótulo.

Rotina para que se posicione o sexto rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 400 pixels para a coordenada X1 deste sexto rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 970 pixels para a coordenada Y1 deste sexto rótulo.
  Atribua o sexto nome ao nome deste sexto rótulo.
  Exiba o sexto rótulo.

Rotina para que se posicione o sétimo rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 800 pixels para a coordenada X1 deste sétimo rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 970 pixels para a coordenada Y1 deste sétimo rótulo.
  Atribua o sétimo nome ao nome deste sétimo rótulo.
  Exiba o sétimo rótulo.

Rotina para que se posicione o oitavo rótulo:
  Atribua a coordenada X1 desta caixa desta tela 
  mais 1200 pixels para a coordenada X1 deste oitavo rótulo.
  Atribua a coordenada Y1 desta caixa desta tela 
  mais 970 pixels para a coordenada Y1 deste oitavo rótulo.
  Atribua o oitavo nome ao nome deste oitavo rótulo.
  Exiba o oitavo rótulo.


O primeiro rótulo é um rótulo.
O segundo rótulo é um rótulo.
O terceiro rótulo é um rótulo.
O quarto rótulo é um rótulo.
O quinto rótulo é um rótulo.
O sexto rótulo é um rótulo.
O sétimo rótulo é um rótulo.
O oitavo rótulo é um rótulo.

O valor da enumeração RotateNoneFlipNone é um número igual a 0.
O valor da enumeração Rotate180FlipXY é um número igual a 0.
O valor da enumeração RotateNoneFlipNone é um número igual a 1.
O valor da enumeração Rotate270FlipXY é um número igual a 1.
O valor da enumeração Rotate180FlipNone é um número igual a 2.
O valor da enumeração RotateNoneFlipXY é um número igual a 2.
O valor da enumeração Rotate270FlipNone é um número igual a 3.
O valor da enumeração Rotate90FlipXY é um número igual a 3.
O valor da enumeração RotateNoneFlipX é  um número igual a 4.
O valor da enumeração Rotate180FlipY é um número igual a 4.
O valor da enumeração Rotate90FlipX é um número igual a 5.
O valor da enumeração Rotate270FlipY é um número igual a 5.
O valor da enumeração Rotate180FlipX é um número igual a 6.
O valor da enumeração RotateNoneFlipY é um número igual a 6.
O valor da enumeração Rotate270FlipX é um número igual a 7.
O valor da enumeração Rotate90FlipY é um número igual a 7.

O primeiro nome é uma string igual a "valor da enumeração RotateNoneFlipNone/Rotate270FlipXY".
O segundo nome é uma string igual a "valor da enumeração Rotate90FlipX/Rotate270FlipY".
O terceiro nome é uma string igual a "valor da enumeração RotateNoneFlipY/Rotate180FlipX".
O quarto nome é uma string igual a "valor da enumeração RotateNoneFlipXY/Rotate180FlipNone".
O quinto nome é uma string igual a "valor da enumeração Rotate90FlipY/Rotate270FlipX".
O sexto nome é uma string igual a "valor da enumeração Rotate90FlipXY/Rotate270FlipNone".
O sétimo nome é uma string igual a "valor da enumeração RotateNoneFlipNone/Rotate180FlipXY".
O oitavo nome é uma string igual a "valor da enumeração RotateNoneFlipX/Rotate180FlipY".
```

O resultado do programa é este:

<div data-full-width="true">

<figure><img src="../.gitbook/assets/RotateFlip.png" alt=""><figcaption></figcaption></figure>

</div>

