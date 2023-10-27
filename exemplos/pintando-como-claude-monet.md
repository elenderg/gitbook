# Pintando como Claude Monet

O programa abaixo utiliza a API do Google para transformar as thumbnails das imagens em pinturas que replicam o estilo de Claude Monet.

```
A caixa de status é uma estrutura com 
  Uma caixa e 
  Uma string.

O campo de texto é uma estrutura com 
  Uma caixa e 
  Uma string.

Um botão é uma estrutura com
  Uma caixa e 
  Um nome.

O botão de imprimir é um botão.
O botão de fechar é um botão.

Uma obra de arte é uma lista com 
  Uma URL e 
  Uma pintura.

A obra de arte atual é um obra de arte.
As obras de arte são umas obras de arte.

Um pintura é uma imagem.
O plano de fundo é uma imagem.

Rotina para que se execute o programa:
  Inicialize os componentes.
  Inicialize a interface.
  Execute os eventos.
  Libere os recursos alocados na memória.
  Feche o programa.

Rotina para que se inicialize a interface:
  Crie o plano de fundo.
  Inicialize a caixa de status.
  Inicialize os botões.
  Inicialize o campo de texto.
  Exiba "Olá Mundo!" na caixa de status.
  Escreva "Debug: Componentes inicializados." para StdOut.
  Escreva na próxima linha da saída padrão.

Rotina para que se crie o plano de fundo:
  Pinte a caixa desta tela com a cor branca e a cor branca.
  Itere.
    Escolha aleatoriamente uma localização no interior de a caixa desta tela.
    Escolha aleatoriamente uma cor entre a cor cinza claríssimo e a cor branca.
    Pincele a cor sobre a localização.
    Se um contador estiver ultrapassando 80000,
      Pare.
    Se o contador for uniformemente divisível por 10000, 
      Atualize a tela.
  Reitere.
  Extraia o plano de fundo usando a caixa desta tela. \ou Crie o plano de fundo desde o tela.

Rotina para que se pincele uma cor sobre uma localização:
  Escolha aleatoriamente o canto superior esquerdo duma elipse dentre 6 pixels de_ a localização.
  Escolha aleatoriamente o canto inferior direito desta elipse dentre 6 pixels de_ a localização.
  Pinte a elipse com a cor.

Rotina para que se inicialize a caixa de status:
  Atribua o centro desta tela para uma localização.
  Atribua a coordenada X desta localização menos 400 pixels para a coordenada X1 desta caixa de status.
  Atribua a coordenada X desta localização mais 400 pixels para a coordenada X2 desta caixa de status.
  Atribua a coordenada Y2 desta tela menos 80 pixels para a coordenada Y1 desta caixa de status.
  Atribua a coordenada Y2 desta tela menos 48 pixels para a coordenada Y2 desta caixa de status.

Rotina para que se inicialize os botões:
  Atribua a coordenada Y2 desta tela menos 48 pixels para a coordenada Y duma localização.
  Atribua a coordenada X2 desta tela menos 48 pixels para a coordenada X desta localização.
  Faça o botão de fechar usando o localização e " Fechar ".
   Atribua a coordenada X1 deste botão de fechar menos 48 pixels para a coordenada X desta localização.
  Faça o botão de imprimir usando a localização e " Imprimir ".

Rotina para que se faça um botão usando uma localização e um nome:
  Atribua a coordenada X desta localização menos a largura deste nome para a coordenada X1 deste botão.
  Atribua a coordenada Y desta localização menos 30 pixels para a coordenada Y1 deste botão.  
  Atribua o localização para o canto inferior direito deste botão.
  Atribua o nome para o nome deste botão.

Rotina para que se inicialize o campo de texto:
  Atribua a coordenada X1 desta tela mais 48 pixels para a coordenada X1 deste campo de texto.
  Atribua a coordenada X1 deste campo de texto mais 300 pixels para a coordenada X2 deste campo de texto.
  Atribua a coordenada Y2 desta tela menos 80 pixels para a coordenada Y1 deste campo de texto.
  Atribua a coordenada Y2 desta tela menos 48 pixels para a coordenada Y2 deste campo de texto.

Rotina para que se exiba uma string na caixa de status: \ TODO: com uma cor
  Atribua a string para a string desta caixa de status.
  Exiba os componentes e atualize a tela.

Rotina para que se exiba os componentes e atualize a tela:
  Oculte o cursor.
  Pinte o plano de fundo.
  Pinte a caixa de status.
  Pinte o botão de imprimir.
  Pinte o botão de fechar.
  Pinte o campo de texto.
  Pinte a obra de arte atual.
  Atualize o tela.

Rotina para que se pinte a caixa de status:
  Pinte a caixa desta caixa de status com a cor preta e a cor cinza claro.
  Pinte a string desta caixa de status no centro de a caixa desta caixa de status com a cor preta.

Rotina para que se pinte uma string em uma caixa no centro:
  Pinte a string na caixa usando "centralizado".

Rotina para que se pinte um botão:
  Pinte a caixa deste botão com a cor preta e a cor cinza claro.
  Pinte o nome deste botão na caixa deste botão com a cor preta.

Rotina para que se pinte o campo de texto:
  Pinte a caixa deste campo de texto com a cor preta e a cor cinza claro.
  Atribua a string deste campo de texto seguido de "_" para uma string.
  Pinte a string na caixa deste campo de texto.

Rotina para que se pinte uma obra de arte:
  Se a obra de arte for inexistente, retorne.
  Se a obra de arte não estiver concluída, retorne.
  Pinte a caixa desta obra de arte com a cor branca e a cor branca.
  Pinte a pintura desta obra de arte.

Rotina para que se execute os eventos:
    Aguarde por um evento.
    Se o evento for inexistente, retorne.
    Execute o evento.
  Reitere.

Rotina para que se execute um evento:
  Se a categoria deste evento for "movimentação de cursor", 
    Execute o evento (movimentação de cursor); 
    Retorne.
  Se a categoria deste evento for "atualização de tela",
    Execute o evento (atualização de tela); 
    Retorne.
  Se a categoria deste evento for "clique do botão esquerdo", 
    Execute o evento (clique do botão esquerdo); 
    Retorne.
  Se a categoria deste evento for "pressionamento de tecla", 
    Execute o evento (pressionamento de tecla); 
    Retorne.

Rotina para que se execute um evento (movimentação de cursor):
  Mostre a seta do mouse.

Rotina para que se execute um evento (atualização de tela):
  Exiba os componentes e atualize a tela.

Rotina para que se execute um evento (clique do botão esquerdo):
  Limpe a caixa de status.
  Se a localização deste evento estiver no botão de imprimir, 
    Imprima a obra de arte.
  Se a localização deste evento estiver no botão de fechar, 
    Saia do programa.

Rotina para que se determine se um localização está em um botão:
  Se a localização estiver na caixa deste botão, diga sim.
  Diga não.

Rotina para que se imprima a obra de arte:
  Se a obra de arte atual for inexistente, 
    Avise o usuário;
    Retorne.
  Exiba "Imprimindo..." na caixa de status.
  Escreva "Debug: Imprimindo..." para StdOut.
  Escreva na próxima linha da saída padrão.
  Inicie a impressão.
  Selecione uma folha para impressão.
  Centralize a pintura desta obra de arte atual na folha.
  Pinte a pintura desta obra de arte atual.
  Centralize a pintura desta obra de arte atual na caixa desta tela.
  Salve as alterações pendentes na folha.
  Acabe de imprimir.
  Exiba "Impressão concluída" na caixa de status.
  Escreva "Impressão concluída..." para StdOut.
  Escreva na próxima linha da saída padrão.

Rotina para que se saia do programa:
  Delegue o controle.

Rotina para que se execute um evento (pressionamento de tecla):
  Limpe a caixa de status.
  Se o evento foi alterado, 
    Execute o evento (Tecla modificadora); 
    Retorne.
  Se o byte deste evento for imprimível, 
    Execute o evento (exibição de caractere); 
    Retorne.
  Atribua a tecla deste evento para uma tecla.
  Se a tecla deste evento for a Tecla Esc, 
    Execute o evento (Tecla Esc); 
    Retorne.
  Se a tecla deste evento for a Tecla Backspace, 
    Execute o evento (backspace); 
    Retorne.
  Se a tecla deste evento for a Tecla Enter, 
    Execute o evento (Tecla Enter); 
    Retorne.
  Se a tecla deste evento for a Tecla Home, 
    Execute o evento (Tecla Home); 
    Retorne.
  Se a tecla deste evento for a Tecla End, 
    Execute o evento (Tecla End); 
    Retorne.
  Se a tecla deste evento for a Tecla Page Up, 
    Execute o evento (Tecla Page Up); 
    Retorne.
  Se a tecla deste evento for a Tecla Page Down, 
    Execute o evento (Tecla Page Down); 
    Retorne.

Rotina para que se execute um evento (Tecla modificadora):
  Se a tecla deste evento for a tecla Q/q, 
    Saia do programa; 
    Retorne.
  Se a tecla deste evento for a tecla P/p, 
    Imprima a obra de arte; 
    Retorne.

Rotina para que se execute um evento (exibição de caractere):
  Acrescente o byte deste evento para a string deste campo de texto.
  Exiba os componentes e atualize a tela.

Rotina para que se execute um evento (tecla Esc):
  Limpe a string deste campo de texto.
  Exiba os componentes e atualize a tela.

Rotina para que se limpe a caixa de status:
  Limpe a string desta caixa de status.
  Exiba os componentes e atualize a tela.

Rotina para que se execute um evento (backspace):
  Se a string deste campo de texto estiver em branco, 
    Avise o usuário; 
    Retorne.
  Remova o último caractere desde a string deste campo de texto.
  Exiba os componentes e atualize a tela.

Rotina para que se execute um evento (tecla Enter):
  Se a string deste campo de texto estiver em branco, 
    Avise o usuário; 
    Retorne.
  Exiba "Aguarde..." na caixa de status.  
  Escreva "Debug: Tecla Enter pressionada. Aguarde..." para StdOut.
  Escreva na próxima linha da saída padrão.
   Atribua "http://images.google.com/images?q=" para um URL.
  \Atribua "http://images.google.com/images?safe=active&q=" para uma URL.
  Converta a string deste campo de texto para um texto de consulta.
  Acrescente o texto de consulta para a URL.
  Leia a URL para um trecho.
  Se o erro do fluxo de entrada/saída não estiver em branco, 
    Exiba o erro do fluxo de entrada/saída na caixa de status; 
    Escreva o erro do fluxo de entrada/saída para StdOut; 
    Escreva na próxima linha da saída padrão;
    Retorne.
  Crie o obras de arte usando o trecho.
  Se as obras de arte estiverem vazias, 
    Exiba "Erro. Não foi possível efetuar a pintura a partir dos termos informados" na caixa de status; 
    Escreva "Erro. Não foi possível efetuar a pintura a partir dos termos informados" para StdOut; 
    Retorne.
  Vá para a primeira obra de arte destas obras de arte.

Rotina para que se crie umas obras de arte usando um trecho:
  Se a quantidade de caracteres deste trecho for 0, 
    Escreva "Erro. O trecho está vazio." para StdOut;
    Escreva na próxima linha da saída padrão;
    Retorne.
  Destrua as obras de arte.
  Atribua inexistente para a obra de arte atual.
  Lance um percorredor sobre o trecho.
  Itere.
    Mova o percorredor (utilizando as diretrizes do Google Imagens).
    Se o segmento inicial deste percorredor estiver em branco, 
      Retorne.
    Escreva o segmento inicial deste percorredor para StdOut.
    Crie uma obra de arte usando o segmento inicial deste percorredor.
    Acrescente a obra de arte para o obras de arte.
  Reitere.

Rotina para que se mova um percorredor (utilizando as diretrizes do Google Imagens):
  Limpe o segmento inicial deste percorredor.
  Itere.
    Se o segmento final deste percorredor estiver em branco, 
      Retorne.
    Se o segmento final deste percorredor começar com "src=""http://t", 
      Pare.
    Adicione 1 para o caractere inicial deste segmento final deste percorredor.
  Reitere.
  Atribua "src=""" para uma string.
  Adicione 5 para o caractere inicial deste segmento final [final] deste percorredor.
  Posicione o segmento inicial deste percorredor sobre o segmento final deste percorredor.
  Mova o percorredor (usando diretrizes de elementos HTML).

Rotina para que se mova um percorredor (usando diretrizes de elementos HTML):
    Se o segmento final deste percorredor estiver em branco, retorne.
    Se o conteúdo deste caractere inicial deste segmento final deste percorredor for o sinal maior do que, retorne.
    Se o conteúdo deste caractere inicial deste segmento final deste percorredor for a aspa dupla direita, retorne.
    Avance o percorredor.
  Reitere.

Rotina para que se crie uma obra de arte usando um URL:
  Aloque memória para a obra de arte.
  Atribua o URL para a URL desta obra de arte.

Rotina para que se vá para um obra de arte:
  Se a obra de arte for inexistente, retorne.
  Exiba "Aguarde um momento..." na caixa de status.
  Escreva "Debug: procurando próxima imagem..." na caixa de status.
  Escreva na próxima linha da saída padrão.
  Atribua a obra de arte para a obra de arte atual.
  Conclua a obra de arte atual.
  Limpe a caixa de status.
  Exiba os componentes e atualize a tela.

Rotina para que se conclua uma obra de arte:
  Se a obra de arte for inexistente, retorne.
  Se a obra de arte estiver concluída, retorne.
  Crie uma imagem usando a URL desta obra de arte.
  Se a imagem for inexistente, 
    \Avise o usuário;
    Exiba "Erro ao encontrar imagem" na caixa de status;
    Escreva "Erro ao encontrar imagem" para StdOut;
    Escreva na próxima linha da saída padrão;
    Retorne.
  Redimensione a imagem para 528 pixels por 528 pixels.
  Centralize a imagem na caixa desta tela.
 Pinte o plano de fundo.
  Pinte a imagem.
  Atribua 0 para um contador.
  Itere.
    Escolha aleatoriamente um localização nas proximidades de a caixa desta imagem.
    Misture uma cor usando o localização.
    Pincele a cor sobre o localização.
    Adicione 1 para o contador.
    Se o contador for maior do que 20000, pare.
  Reitere.
  Extraia a pintura desta obra de arte usando a caixa desta imagem.
  Destrua a imagem.

Rotina para que se determine se uma obra de arte está concluída:
  Se a obra de arte for inexistente, diga sim.
  Se a pintura desta obra de arte não for inexistente, diga sim.
  Diga não.

Rotina para que se escolha aleatoriamente uma localização nas proximidades de uma caixa:
  Preserve a caixa.
  Recue a caixa usando 8 pixels.
  Escolha aleatoriamente a localização no interior de a caixa. \ noodle

Rotina para que se misture uma cor usando um localização:
  Obtenha o cor usando o localização.
  Se a cor não for alguma cor muitíssimo clara, retorne.
  Escolha aleatoriamente o cor entre a cor cinza claríssimo e a cor branca.

Rotina para que se execute um evento (tecla Home):
  Se a obra de arte atual for inexistente, 
    Escreva "Erro ao encontrar imagem" para StdOut;
    Escreva na próxima linha da saída padrão;
    Avise o usuário; 
    Retorne.
  Se a obra de arte atual for a primeira obra de arte destas obras de arte, 
    Avise o usuário; 
    Retorne.
  Vá para a primeira obra de arte destas obras de arte.

Rotina para que se execute um evento (tecla End):
  Se a obra de arte atual for inexistente,
    Escreva "Erro ao encontrar imagem" para StdOut;
    Escreva na próxima linha da saída padrão;  
    Avise o usuário; 
    Retorne.
  Se a obra de arte atual for a última obra de arte destas obras de arte, 
    Avise o usuário; 
    Retorne.
  Vá para a última obra de arte destas obras de arte.

Rotina para que se execute um evento (Tecla Page Down):
  Se a obra de arte atual for inexistente, 
    Escreva "Erro ao encontrar imagem" para StdOut;
    Escreva na próxima linha da saída padrão;
    Avise o usuário; 
    Retorne.
  Se a próxima obra de arte desta obra de arte atual for inexistente, 
    Avise o usuário; 
    Retorne.
  Vá para a próxima obra de arte desta obra de arte atual.

Rotina para que se execute um evento (Tecla Page Up):
  Se a obra de arte atual for inexistente,
    Escreva "Erro ao encontrar imagem" para StdOut;
    Escreva na próxima linha da saída padrão;  
    Avise o usuário; 
    Retorne.
  Se a obra de arte anterior desta obra de arte atual for inexistente, 
    Escreva "Erro ao encontrar imagem" para StdOut;
    Escreva na próxima linha da saída padrão;
    Avise o usuário; 
    Retorne.
  Vá para a obra de arte anterior desta obra de arte atual.

Rotina para que se libere os recursos alocados na memória:
  Destrua o plano de fundo.
  Destrua o obras de arte.

```

Outputs produzidos pelo programa:



<div>

<figure><img src="../.gitbook/assets/jardim florido.PNG" alt=""><figcaption><p>Jardim Florido</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/octocat.PNG" alt=""><figcaption><p>Octocat</p></figcaption></figure>

 

<figure><img src="../.gitbook/assets/Paisagem.PNG" alt=""><figcaption><p>Paisagem</p></figcaption></figure>

</div>
