---
layout: post
current: post
navigation: True
title: Escolhendo um framework mobile em 2019
date: 2019-04-15 10:18:00
tags: mobile
class: post-template
subclass: 'post tag-mobile'
author: leandro
excerpt:  Com tantas opções, como escolher um framework mobile em 2019?
meta-description: Com tantas opções, como escolher um framework mobile em 2019?
cover: False
comments: false
---

Com tantas opções, como escolher um framework mobile em 2019?

---

Antes, tínhamos poucas opções e era claro qual caminho seguir. Em 2019 temos tantas opções que é preciso perguntar:

* **O que usar?**

Essa pergunta foi feita tantas vezes que ela mesmo já está cansada. Mas a resposta não é óbvia. Para responder precisamos refletir sobre outras questões.

## Qual a natureza e complexidade do aplicativo?

Aplicativos diferentes requerem coisas diferentes, então é importante dar aquela pensada: *na linguagem que eu vou escolher é possível fazer as coisas que quero fazer?*

É claro que pra responder isso você precisa saber **o que você quer fazer**. Se você não sabe, talvez vale a pena voltar pra lousa e dar uma rabiscada na ideia principal.

Eu vou construir um cronômetro que eventualmente vai se comunicar com um servidor para gravar as estatísticas do usuário. 

Então, um contador de tempo que faz umas chamadas web. Numa escala *Bighetti’s Complexity Scale* ® eu diria médio. Melhor descrito como *nada muito doido*.

## Você precisa de iOS ou Android? Ou ambas?

Quais plataformas? As soluções podem variar dependendo da resposta.

Meu público alvo é Android então foquei apenas nesse sistema operacional, mas fiquei aberto a outras possibilidades.

## Qual a preferência dos desenvolvedores?

Uma prioridade minha é **otimizar para felicidade**. Se o você é absolutamente miserável utilizando uma linguagem ou tecnologia… por que usá-la?

Porque usar uma coisa que você não gosta?
> Mas eu não tenho escolha, eu tenho que usar esta tecnologia.

Eu entendo, às vezes precisamos pagar as contas ou engolir uns sapos. É a vida. Mas tenha em mente que uma pessoa utilizando algo que não gosta é uma pessoa **improdutiva**. Em contraste, uma pessoa entusiasmada é uma pessoa extremamente produtiva. E, como diz o [DHH](https://twitter.com/dhh), criador do Ruby on Rails:
> ## Não é possível fingir entusiasmo.

Antes de ir para Elixir e Elm, eu trabalhei com Java e Javascript por 5 anos.

Quando mudei, passei a amar programação funcional, a ser mais feliz e mais produtivo usando linguagens funcionais. Principalmente mais feliz. Muito mais feliz. Incrivelmente mais feliz.

![](https://media.giphy.com/media/B0vFTrb0ZGDf2/giphy.gif)

E por isso, nesta busca de uma solução para desenvolvimento mobile, a primeira coisa que fui buscar foram soluções que envolviam programação funcional.

Vamos então a minha saga.

## Take 1: Elm Native UI

![](https://cdn-images-1.medium.com/max/2000/1*euxL76LFub9ZR-YdYlWNEA.png)

Eu trabalho diariamente com Elm no frontend.

Elm é de longe a melhor experiência de frontend que eu tive nos últimos 7 anos.

Elm é absolutamente incrível: rápido, produtivo e legível. Um compilador que praticamente te carrega no colo e claro, zero erros de runtime.

Se o programa compila, não dá erro. Simples assim. Dar manutenção pra um base de código em Elm é maravilhoso.

Ter essas coisas no desenvolvimento mobile seria um sonho. Infelizmente ainda é apenas isso, um sonho.

Elm Native é um projeto separado, não tem conexão e não é desenvolvido pelos mesmos desenvolvedores do Elm. O desenvolvimento era feito por uma única pessoa que não dá mais manutenção. Em produção, achei apenas um único uso.

Elm Native compila pra React Native, coisa que é bem diferente do que o Elm original faz e contém bugs independentes que provavelmente não vão ser corrigidos num futuro próximo.

A idéia é maravilhosa, mas infelizmente eu achei que ainda não valeria o investimento. Quem sabe um dia?

## Take 2: Lambda Native

![Estudo comparando horas de desenvolvimento mobile — Java vs C/C++ vs Scheme](https://cdn-images-1.medium.com/max/3084/1*mHmR1Qb78xSuNouED7sxlw.jpeg)*Estudo comparando horas de desenvolvimento mobile — Java vs C/C++ vs Scheme*

Esse projeto vem no topo das buscas se você pesquisar por linguagem funcional e mobile e eu no entanto eu nunca tinha ouvido falar dele. A linguagem usada é Scheme, um dialeto de Lisp.

O principal ponto parece ser a velocidade de desenvolvimento. Eles citam um estudo onde um mesmo aplicativo foi criado com Scheme 10x mais rápido que com Java. Impressive.

Os exemplos são legais e tem pouquíssimas linhas. Parece também estar sendo usado em faculdades.

Pra essa opção, eu resolvi dar um passo pra trás pelo seguinte: eu trabalho com Elixir e Elm, eu tento dedicar meus esforços de estudo a essas linguagens. Eu sou um desenvolvedor horrendo de Lisp, eu precisaria de um esforço homérico pra compreender o que se passa aqui.

Analise esse hello world por exemplo:

<script src="https://gist.github.com/lbighetti/1e6b18cdc190eb32ec063e67198dcbf8.js"></script>

Se o código acima é legível pra você, essa solução pode ser uma boa tentativa. Para mim é quase uma comunicação alienígena. 👽

Compare com o hello world em Elm:

<script src="https://gist.github.com/lbighetti/587e150c1701bdd0356631853806775a.js"></script>

Eu achei a complexidade e o esforço que eu teria que dedicar muito grande pra uma projeto pessoal.

Isso me fez considerar um outro fator: reutilizar coisas que eu já sei. Como eu disse um pouco acima, anteriormente eu era desenvolvedor Java. Porque não tentar a solução padrão de Java com Android?

## Take 3: Android com Java

![Android segurando a xícara de Java](https://cdn-images-1.medium.com/max/2000/1*Hgst6lyMx05LclZjYMr12w.jpeg)*Android segurando a xícara de Java*

Já faziam 2 anos que não mexia com Java, mas foi como andar de bicicleta.

Utilizar o Android Studio, que é uma versão modificada do IntelliJ, foi uma surpresa agradável. Eu adoro o IntelliJ. Apesar disso, eu não gosto de estar preso a uma IDE. Desenvolver fora do Android Studio é um pesadelo. Eu acho isso conceitualmente ruim. Te deixa empacado ali sem opção.

Mas deveras, a experiência no Android Studio é muito boa. A instalação é fácil e ele vai te dando as dicas do que fazer. Tem *wizard* pra tudo, e com alguns cliques você sai com oOlá Mundo rodando.

No meu TCC em 2013 fiz um app Android e a experiência na época era lamentável. O jeito era usar um plugin bugado do Eclipse que dava crash a cada 15 minutos e um emulador comia 90% do seu CPU. Foi bom ver que as evoluíram por aqui.

Mas uma parte me deu um soco no estômago.

Os layouts são editados em XML.

XML.

X.
M.
L.

**Em 2019.**

Não pode ser.

Meu coração se quebrou como se tivesse terminado um namoro.

Busquei como fazer layouts sem XML, e dá, mas a solução é ruim. O código vira uma várzea.

Daí me veio uma luz na escuridão… lembrei do Kotlin!

## Take 4: Android com Kotlin

![Kotlin logo](https://cdn-images-1.medium.com/max/2000/1*er4JB9GyUElrZ1f4KmPYQA.png)*Kotlin logo*

Kotlin é uma linguagem que roda na JVM (a máquina virtual do Java) e é desenvolvido pela JetBrains, a empresa que faz o IntelliJ. Eles mandam muito bem, sabem o que tão fazendo.

O Kotlin é o que muita gente gostaria que o Java fosse.

Pra melhorar, o Google anunciou que Kotlin é oficialmente suportada pra Android.

E… o logo deles é muito bonito. Sério. É o logo mais bonito que eu já vi.

Comecei o que tinha feito com Java, dessa vez em Kotlin, e foi tudo suave. Kotlin é uma boa linguagem. Joga tudo que não presta do Java fora e melhora as melhores partes. É mais legível, mais fácil de manter e mais rápido de desenvolver. O que você faz com Java no Android Studio, você faz também com Kotlin sem dificuldade.

No geral, a solução é muito boa. Mas… O meu nêmesis do XML ainda continua o mesmo.

Se você consegue tolerar o XML, eu recomendo tentar esta solução porque Kotlin é uma linguagem excelente e a integração com o Android Studio é perfeita.

Eu decidi que eu não tenho estômago pra isso em 2019 e resolvi continuar a minha busca.

Nisso, cai num framework chamado Anko.

## Take 5: Android com Kotlin e Anko



![Android com bandeiras de Kotlin](https://cdn-images-1.medium.com/max/3000/1*J9C7HXwLafBDpROhUP0vxw.png)*Android com bandeiras de Kotlin*

Anko é um framework desenvolvido pela JetBrains que usa código Java ao invés de XML para o layout.

Perfeito!

Tentando um olá mundo me deparei com exemplo desatualizado. O build não rodava por ter uma versão muito velha, mas ao tentar atualizar para uma mais nova dava erro de compilação. Bleh.

Na documentação do setup manual, de novo documentação desatualizada e coisas antigas que não funcionavam mais.

No fim das contas consegui fazer o setup funcionar, mas a experiência foi bem longe de ideal.

O problema aqui é que a JetBrains deixou apenas **um único desenvolvedor** responsável pelo projeto, e quando questionada sobre a falta de progresso, responderam que o desenvolvedor tem outras prioridades no momento.

¯\_(ツ)_/¯

Esse setup era o mais promissor pra mim. Kotlin com Anko tinha o potencial de fazer a JetBrains dominar esse mercado. Eles estavam com a faca e o queijo na mão, jogaram o queijo no chão e enfiaram a faca no c*.

Mas… parei de insistir, e resolvi tentar algo completamente novo.

O Flutter.

## Take 6: Flutter

![](https://cdn-images-1.medium.com/max/3840/1*wKjksVGC0c8haaV3-kWMCg.png)

Flutter é um garoto novo na quebrada e tem potencial.

Um framework desenvolvido pelo Google que visa unificar o desenvolvimento mobile, criar interfaces bonitas via código e ser fácil de manter. Isso além de ser *cross-platform*, isso é, compila tanto para Android quanto para iOS.

Logo na instalação já fui surpreendido com uma documentação maravilhosa, dando um passo a passo que até um macaco poderia seguir. Atualizada e precisa. *Boom!*

O Flutter utiliza a instalação do Android Studio, mas torna as funcionalidades independentes do editor. Ele faz isso criando ferramentas *cli* pra linha de comando.

Ou seja, você pode utilizar o Android Studio (Ou o VSCode) como editor se quiser, mas pode também fazer tudo pela linha de comando e ficar livre pra usar qualquer editor quiser.

E a linha de comando funciona que é uma beleza! O flutter doctor vai te guiando, passo a passo, e dá sugestões de como arrumar os problemas.

Essa experiência foi infinitamente melhor do que ficar lutando contra uma IDE pra resolver problemas.

Pra começar um projeto do zero você pode utilizar o flutter create, similar ao rails new do Rails ou mix newdo Elixir.

![](https://cdn-images-1.medium.com/max/5300/1*QCajckOeBhRaLzi0RoFqig.png)

A linguagem de programação usada pelo Flutter é o Dart, também desenvolvido pelo Google. Inicialmente eu não dei nada pro Dart, mas depois de usar ele um pouco, senti que ele é ergonômico, não entra na sua frente, consegue entregar o que se propõe e é fácil de ler. Nesses quesito eu vi que é similar ao Kotlin, pegando bons aspectos de orientação a objetos (OO) e jogando outros fora. Porém, diferente do Kotlin, usando Dart você sente que **não** está no ecossistema JVM, apesar de ter a ponta do Android.

Ainda assim, eu não amo Dart de paixão como Elixir ou Elm, mas ele entrega o que promete e pro momento isso é suficiente.

Em poucos minutos eu estava debugando meu olá mundo no celular, e foi aí que me veio outra surpresa agradável.

O Flutter tem uma funcionalidade chamada **hot reload**. Ela faz com que código novo seja atualizado no aplicativo rodando em tempo real! Você troca o layout da tela e o app no celular atualiza na hora. Já estamos mimados e acostumados a ter isso para web, mas para mobile não é a norma.

Tipicamente em Android ou iOS você tem que reinstalar o seu pacote para ver as mudanças e perde muito tempo com isso. Aqui não. Mudou, deu live-reload, app atualizado enquanto roda. Simplesmente maravilhoso.

Pra finalizar, o gigante Google tem um time dedicado desenvolvendo Flutter e Dart, e isso fica bem claro pela alta qualidade de todo o ecossistema, atualizações de bug fixes e melhorias.

Se olharmos o resumo do último mês no repositório do GitHub deles, eles tem _267 Pull requests aceitos por 58 pessoas. **Insano**._

![](https://cdn-images-1.medium.com/max/3048/1*gl9Pwr3v1ibiiJ9mGvWWbg.png)

A cereja no topo do bolo: tudo open source.

Em outras palavras:

* documentação excelente

* facilidade de instalação

* ferramentas de linha de comando

* independência de editor/ide

* linguagem razoável

* hot reload

* open source

* time dedicado desenvolvendo

Então, tomei minha decisão.

Vou usar **Flutter**.

## Mas e React Native, Ionic, Xamarin, insira framework ______?

Eu julguei que Flutter é a melhor opção **pra mim**, diante do meu caso de uso, da minha preferência e das minhas habilidades.

Mas isso não quer dizer que é a melhor opção **pra você**. Existem outras opções nesse mundão afora.

Por exemplo, se você gosta de Javascript, Ionic e React Native são frameworks que você deveria considerar. Eles são *cross-platform* e tem muita gente usando, de pequenos a enormes casos de uso.

Pra mim não faz sentido. Eu não gosto de Javascript. A vida é assim, algumas pessoas gostam de azul outras de vermelho.

**E tudo bem**. Não tem problema.

Xamarin, C#, mesma coisa. Ótimo framework, ótima linguagem, mas não é pra mim.

## Conclusão

Em 2019, desenvolver um app mobile é talvez mais fácil do que nunca, e ao mesmo tempo o grande número de framework pode nos deixar paralisados(as).

Minha estratégia foi explorar soluções que achei que faziam sentido, dado o meu contexto. Nem de perto explorei todas elas, apenas um número razoável, e escolhi a que melhor me identifiquei.

Minha escolha, foi o Flutter. Pontos que me ganharam: um setup fácil e layout em código. Pontos bônus: debug no celular com *hot reload *e liberdade de usar qual editor eu quiser.

E você? Qual a sua  escolha? Me manda lá no twitter pra gente comparar as experiências!
https://twitter.com/leandrobighetti

Obrigado por sobreviver até aqui e até a próxima!
