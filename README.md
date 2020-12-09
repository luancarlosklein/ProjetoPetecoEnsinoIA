# Grupo de Pesquisa em Sistemas Multiagente do PETECO
Projeto de Ensino da UTFPR do PETECO-Curitiba que visa o ensino de aspectos de Inteligência Artificial com o objetivo de preparação para a realização de pesquisa científica. O tema principal de enfoque desse projeto são Sistemas Multiagente.

Este projeto está dividido inicial em 3 tópicos principais de ensino: Básico, Intermediário e final.
Diversas atividades serão feitas ao longo dessa atividade.
O projeto final de validação será um sistema completo envolvendo todos os aspectos estudados. O exemplo dele está disponível em: https://github.com/luancarlosklein/TruckProjectMAS, que foi desenvolvido como trabalho principal de IC pelo aluno Luan Carlos Klein em conjunto com o professor orientador Cesar Augusto Tacla.

## Parte 1: Básico

- Conceitos Fundamentais
  - Agentes
    - Conceito básico de agentes: Um agente é um sistema computacional que apresenta as propriedades que seguem. Autonomia: é a capacidade de operar de maneira independente com o mínimo de interferência humana. Habilidade social: é a capacidade de interagir com outros agentes por meio de uma linguagem de comunicação. Reatividade: é a capacidade de perceber mudanças no ambiente e responder em tempo hábil. Proatividade: é a capacidade de exibir comportamentos direcionados a metas por iniciativa própria (Fonte: Wooldridge, M. (2009).An introduction to multiagent systems. John Wiley & Sons, Capitulo 1 Programming  multi-agent systems in AgentSpeak using jason).
  
 - Tipos de ambiente e suas características: 
 [Conceitos Resumidos](https://github.com/luancarlosklein/ProjetoPetecoEnsinoIA/blob/master/Introducao-agentes-ambientes.pdf)
  
- Modelo BDI
  - O modelo BDI define a modelagem de estados mentais através de Beliefs, Desires and Intentions (Crenças, Desejos e intençõoes). (Fonte: Georgeff, M., Pell, B., Pollack, M., Tambe, M., and Wooldridge, M. (1998).  The belief-desire-intention model of agency.  InInternational workshop on agent theories, archi-tectures, and languages, pages 1–10. Springer-Verlag, London, UK., Capitulo 2 Programming  multi-agent systems in AgentSpeak using jason).

- Introdução JASON
  - O JASON é uma ferramenta na qual podemos criar e modelar agentes (baseado no modelo BDI), definindo suas crenças, objetivos e planos. Além disso, ele possibilita realizar interações entre os agentes e o ambiente, além de muitas outras coisas. O JASON será nossa principal ferramenta de uso. Inicialmente não se preocupe com a parte gráfica (mais a frente veremos com calma isso). Nosso grande manual será o livro: Bordini,  R.  H.,  H ̈ubner,  J.  F.,  and  Wolldridge,  M.  (2007). Programming  multi-agent systems in AgentSpeak using jason, volume 1. John Wiley & Sons ltd. 

  - Por questões de facilidade no uso e na integração de ferramentas, utiliza-se a [IDE Eclipse](https://www.eclipse.org/downloads/). Uma vez feita a instalação do mesmo, siga esse tutorial para a instalação do plugin do [JASON](http://jason.sourceforge.net/mini-tutorial/eclipse-plugin/). OBS: Essa parte é MUITO importante. É necessário que tudo esteja certo e funcionando, para podermos aplicar os conhecimentos na prática.

  ### Atividade 1
  - Leia e faça alguns exercícios dos capitulos: 3, 4, 5 e 6 do livro do Bordini. 
  
    - Alguns aspectos importantes que serão aprendidos nos capítulos da leitura:
      - Como é feita a programação em Jason e qual é o "paradigma" utilizado por ele;
      - Como funciona a execução e o raciocinio dos agentes no Jason;
      - O que são os ambientes;
      - Comunicação entre agentes (Atenção especial ao CNP-> Contract Net Protocol).
  
  - Se tiver alguma duvida em algum exercício, ou quiser comparar suas soluções, nesse [link](http://jason.sourceforge.net/jBook/jBook/Examples.html), há algumas soluções que podem ser úteis.
  
- Introdução JAVA
  - Caso você já tenha conhecimento na linguagem JAVA, pode ignorar essa parte. Do contrário, é interessante já ir conhecendo e se adaptando, pois mais para frente, utilizaremos ele para realizar muitas coisas. Um dos tutorias para aprender [JAVA](link). 
  
- Exemplo prático: Beer Robot
  

## Parte 2: Intermediária

Nessa parte, iremos explorar alguns algoritimos famosos, e muito úteis. Atráves deles, vamos dar um pouco mais de "inteligência" aos nossos agentes. Nesse momento, iremos utilizar a linguagem python. Nosso objetivo é entender o funcionamento dos algoritmos, devido a isso, o python pode ser mais rápido e fácil do que fazer isso no JAVA/JASON. 

- Introdução a python
  - Se você já conhece python, fique a vontade para pular essa parte. Se não conhecer, gaste um tempinho aprendendo um pouco. Não precisa nada muito a fundo. O aprendizado pode vir com a prática aqui.

- Por enquanto, vamos focar nos algoritmos de busca de caminhos. Todos os algortimos aqui fazem busca em grafos. Podemos modelar um grafo para representar um grid bidimensional, e esse grid representa o ambiente onde nosso agente está. É muito importante além de aprender os algortimos, fazer alguns questionamentes e tentar entender algumas questões como: No que isso se relaciona com agentes? Quando eu posso usar isso? E quando não posso? Essa pesquisa é feita para um agente sozinho, ou eu poderia fazer com que eles "cooperassem" entre si? E assim segue. É legal pensar nesses pontos. Sem mais delongas, vamos conhecer alguns algortimos. 

  - DFS (Deep First Search - Busca em Profundidade);
  - BFS (Branch Fist Search - Busca em largura);
  - Aprofundamento interativo;
  - A*;
  - Dijkstra;
  - LRTA* (Learning Real Time A*).
  
  Alguns desses tópicos estão disponíveis nos slides do professor Cesar Tacla, nesse [link](https://github.com/luancarlosklein/ProjetoPetecoEnsinoIA/blob/master/Busca-OnLine-DFS-LRTA.pdf).
  É importante ficar claro nesse momento as diferenças entre os algoritmos que funcionam de maneira offline e online.
  
 
- OBS: Além de entender os algoritmos, é fundamental que você implemente todos eles (pode ser em qualquer linguagem inicialmente, o imporntante é entender o que acontece por trás)!!!
 
 <br>
 A segunda parte desse módulo é sobre planejamento. Existem diversos tópicos associados a esse tema. 
 Dentre os temas a serem aprendidos são:
 - O que é Planner?
 - A Linguagem de modelagem (PPDL - Planning Domain Defition Language)
 - SatPlan
 - GraphPlan
 - POP
 - Planning cooperativo

<br> O Material para estudo são os capítulos 10 e 12 do livro do Russel.


Por fim, mas não menos importante, introduzimos as Internal Actions. Elas serão especialmente uteis para colocarmos mais funções e ações nos nossos agentes!
- Leia o capítulo 7 do livro de Bordino.

## Parte 3: Avançado

Nessa parte, iremos ver alguns conceitos importantes e iremos aplicar nossos conhecimentos na prática.

- Reputação e Imagem:
- Parte gráfica no JASON:

## Trabalho Final: Implementação do sistema de descarregamento de caminhões. A especificação sem encontra [aqui](link).


## Extra: Como fazer pesquisa cíentifica

## Próximos passos

Se você completou todos os estágios anteriores e chegou até aqui, parabéns. Nesse momento você está apto para começar a realizar pesquisas.
Lembrando que esse material é apenas para você aprender a "gatinhar". A área de IA está em constante evolução, e diversos conhecimentos são produzidos. Sempre se mantenha atualizado e lembre-se: Aprendizado é uma terefa contínua. 

- Como diz Flávio Augusto (sim, o da Wise-Up): Não é sobre o quanto você sabe, mas sim o que você faz com o que você sabe.

## Temas em aberto para pesquisa

Agora que você já sabe pesquisar, existem divesas áreas em que você pode começar a aplicar seus conhecimentos. 

Algumas delas são:
- RoboFun, do PETECO (UTFPR-Curitiba)
- Iniciação científica

Um dos atigos publicados que resultou dessa pesquisa está disponível em: https://eventos.utfpr.edu.br//sicite/sicite2020/paper/view/5992
E ganhou o prêmio de destaque na área de computação!

