---
description: >-
  O código abaixo demonstra a criação de botões, rótulos e campos de texto, bem
  como gerenciamento de input do usuário.
---

# Exemplo de interface

a

```
Rotina para que se execute o programa:
  Inicialize os componentes.
  Atribua "Lexend" para a fonte padrão.  
  Inicialize a interface.
  Execute os eventos.
  Feche o programa.

Um rótulo é uma estrutura com 
  Uma caixa e 
  Uma string.

O rótulo de e-mail é um rótulo.

Um campo textual é uma estrutura com 
  Uma caixa e 
  Uma string.

O campo de e-mail é um campo textual.

Um botão é uma estrutura com
  Uma caixa e 
  Um nome.

O botão de fechar é um botão.

A localização do botão de fechar é uma localização.

Rotina para que se inicialize a interface:
  Limpe a tela com a cor cinza claríssimo.
  Posicione o rótulo de e-mail.
  Posicione o botão de fechar.
  Faça o botão de fechar usando o localização do botão de fechar e " Fechar ".
  Posicione o campo de e-mail.
  Exiba "Digite o email:" no rótulo de e-mail.

Rotina para que se posicione o rótulo de e-mail:
  Atribua a coordenada X1 desta tela para a coordenada X duma localização.
  Atribua a coordenada Y1 desta tela para a coordenada Y desta localização.
  Atribua a coordenada X desta localização 
    mais 100 pixels para a coordenada X1 deste rótulo de e-mail.
  Atribua a coordenada Y desta localização 
    mais 50 pixels para a coordenada Y1 deste rótulo de e-mail.
  Atribua a coordenada X desta localização 
    mais 250 pixels para a coordenada X2 deste rótulo de e-mail.
  Atribua a coordenada Y desta localização 
    mais 100 pixels para a coordenada Y2 deste rótulo de e-mail.

Rotina para que se posicione o campo de e-mail:
  Atribua a coordenada X1 desta tela para a coordenada X duma localização.
  Atribua a coordenada Y1 desta tela para a coordenada Y desta localização.
  Atribua a coordenada X desta localização 
    mais 280 pixels para a coordenada X1 deste campo de e-mail.
  Atribua a coordenada X desta localização 
    mais 680 pixels para a coordenada X2 deste campo de e-mail.
  Atribua a coordenada Y deste localização 
    mais 60 pixels para a coordenada Y1 deste campo de e-mail.  
  Atribua a coordenada Y desta localização 
    mais 90 pixels para a coordenada Y2 deste campo de e-mail.

Rotina para que se posicione o botão de fechar:
  Atribua a coordenada Y2 desta tela 
    menos 48 pixels para a coordenada Y duma localização.
  Atribua a coordenada X2 desta tela 
    menos 48 pixels para a coordenada X desta localização.
  Atribua a localização para a localização do botão de fechar.
  

Rotina para que se faça um botão usando uma localização e um nome:
  Atribua a coordenada X desta localização 
    menos a largura deste nome para a coordenada X1 deste botão.
  Atribua a coordenada Y desta localização 
    menos 30 pixels para a coordenada Y1 deste botão.  
  Atribua o localização para o canto inferior direito deste botão.
  Atribua o nome para o nome deste botão.

Rotina para que se exiba uma string em um rótulo: \ TODO: com uma cor
  Atribua a string para a string deste rótulo de e-mail.
  Exiba os componentes e atualize a tela.

Rotina para que se exiba os componentes e atualize a tela:
  Oculte o cursor.  
  Pinte o rótulo de e-mail.
  Pinte o botão de fechar.
  Pinte o campo de e-mail.
  Atualize a tela.

Rotina para que se pinte um rótulo:
  Pinte a caixa deste rótulo 
  com a cor cinza claríssimo e a cor cinza claríssimo.
  Pinte a string deste rótulo no centro de 
  a caixa deste rótulo com a cor preta.

Rotina para que se pinte uma string em uma caixa no centro:
  Pinte a string na caixa usando "centralizado".

Rotina para que se pinte um botão:
  Pinte a caixa deste botão com a cor preta e a cor vermelha.
  Pinte o nome deste botão na caixa deste botão com a cor branca.

Rotina para que se pinte o campo de e-mail:
  Pinte a caixa deste campo de e-mail com a cor branca e a cor azul celeste.
  Atribua a string deste campo de e-mail seguido de "_" para uma string.
  Pinte a string na caixa deste campo de e-mail 
  com a cor branca e a fonte padrão e "centralizado".

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
    Se a localização deste evento estiver no botão de fechar, 
      Saia do programa.

Rotina para que se determine se um localização está em um botão:
  Se a localização estiver na caixa deste botão, diga sim.
  Diga não.

Rotina para que se saia do programa:
  Delegue o controle.

Rotina para que se execute um evento (pressionamento de tecla):
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
    Execute o evento (Tecla Esc); 
    Retorne.

Rotina para que se execute um evento (exibição de caractere):
  Acrescente o byte deste evento para a string deste campo de e-mail.
  Exiba os componentes e atualize a tela.

Rotina para que se execute um evento (tecla Esc):
  Delegue o controle.

Rotina para que se limpe um rótulo:
  Limpe a string deste rótulo.
  Exiba os componentes e atualize a tela.

Rotina para que se execute um evento (backspace):
  Se a string deste campo de e-mail estiver em branco, 
    Avise o usuário; 
    Retorne.
  Remova o último caractere desde a string deste campo de e-mail.
  Exiba os componentes e atualize a tela.
```

