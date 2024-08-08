# Evitando problemas de cintilação (Flickering)

Na maioria das vezes, uma exibição de tela completa consiste em vários objetos distintos e sobrepostos, desenhados de trás para frente.

Resolvemos esse problema da mesma forma que um artista faria. Trabalhamos em uma tela na memória (chamada de Contexto de Dispositivo - DC). Esta tela é como se fosse uma tela virtual. Funciona mais ou menos assim: Primeiramente devemos selecionar a área a ser pintada (neste caso queremos pintar em toda a tela, para isso usamos o comando "Exponha tudo". Depois você "pinta" ou "desenha" todas as coisas que deseja nesta tela virtual, e depois disso exibe-a de uma só vez (usando o comando "Atualize a tela").

```
Rotina para que se ececute o programa:
  Carregue as bibliotecas padrão.
  Limpe a tela usando a cor violeta.
  Atribua "https://cdn-icons-png.flaticon.com/512/5332/5332306.png" para uma URL denominada caminho.
  Crie uma imagem usando o caminho.
  Pinte a imagem.
  Atualize a tela.
  Itere.
    \Desenfileire um evento.
    \Se o evento for inexistente, pare.
    \Se a categoria deste evento for "pressionamento de tecla", pare.
    [As linhas acima foram comentadas pois interrompiam a movimentação da imagem]
    Adicione 1 para o contador.
    Mova a imagem 10 pixels para a direita.
    Aguarde 3 milliseconds. 
    Exponha tudo. \ -> Seleciona a tela inteira para ser pintada
    Pinte a caixa desta tela com a cor violeta e a cor violeta.
    Pinte a imagem.
    Atualize a tela.
    Atribua a caixa desta tela à caixa deste contexto.
    Se o contador for 200, pare.
  Reitere.
  Aguarde pela tecla Esc.
  Destrua a imagem.
  Renuncie ao controle.

```

b
