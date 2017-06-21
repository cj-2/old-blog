---
layout: post
title: Pacotão de códigos CSS que você não lembra como se escreve '#01
categories: Pacotão CSS
---

Para começar a primeira série de posts nada melhor do que algo que sempre **quebra sua cabeça.**
Sabe **aquele CSS** que você sempre usa mas não lembra como se escreve?
Pois é, tem uma boa chance dele estar aqui.

Mas se não estiver, paciência. Uma hora sai! (Então salve essa site nos seus favoritos e aproveite.)

## Transition (Efeito de Transição)

    .transition {
      transition: all .3s linear .5s;
    }

**Transition** ou **Transição** é o efeito que está presente nos **links e menus** que ao se passar o mouse ou clicar ocorre um pequeno efeito de mudança de cor, tamanho ou formato.

O primeiro valor **'all'** indica que todas as propriedades irão sofrer o efeito de transição, por exemplo:

    .transition-all{
      transition: all .3s linear;
      background: red;
      color: white;
    }

    .transition-all:hover{
      margin-left: 25px;
      color: black;
      background: yellow;
    }

**Todos os valores** como o background, o color e o margin irão mudar com uma transição de .3s linear.

A propriedade também pode **ser escolhida** e assim excluindo a transição das outras, por exemplo, se eu quisesse que apenas a opacidade mudasse:

    .transition-only-opacity{
      transition: opacity .3s linear .2s;
      background: green;
      color: white;
    }

    .transition-only-opacity:hover{
      margin-left: 25px;
      opacity: 0.5;
    }

O objeto ainda irá se locomover para o lado, **porém** com o **efeito de transição** apenas na opacidade.

O **segundo valor** já é bastante obvio pois se seguir pela lógica vai chegar a conclusão que é o tempo gasto na **transição**, e você está correto.

O **terceiro valor** já não é tão obvio mas nem tão difícil assim, é o tipo de transição (No final desse tópico há um link mais profundo sobre o assunto).

E finalmente o **quarto valor** é a duração do deley (sempre o segundo valor de tempo atribuído), por exemplo:

    .transition-delay{
      transition: all .3s linear .5s;
      background: blue;
      color: white;
    }

    .transition-delay:hover{
      margin-left: 25px;
      background: black;
    }

Os efeitos de transição irão *esperar* .5s para começarem apos a ação (passar o mouse por exemplo).

[Clique aqui](http://liveweave.com/NrbFPA) para ver os exemplos ao vivo e [aqui](https://www.w3.org/TR/css3-transitions/) para saber mais sobre a propriedade transition.
