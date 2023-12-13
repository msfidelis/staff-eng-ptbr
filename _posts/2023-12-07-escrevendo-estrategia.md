---
title: Operando como Staff / Escrevendo uma Estratégia de Engenharia
author: Tao He
date: 2023-12-07
category: OperatingAtStaff
layout: post
mermaid: true
---

> *"Eu meio que acho que escrever sobre estratégia de engenharia é difícil porque uma boa estratégia é bastante entediante, e é meio chato escrever sobre isso. Além disso, eu acho que quando as pessoas ouvem 'estratégia', elas pensam em 'inovação'." - [Camille Fournier](https://twitter.com/skamille/status/1328763503973429250)*

Poucas empresas entendem sua estratégia de engenharia e visão. Uma consequência dessa incerteza é a crença na indústria de que esses documentos são difíceis de escrever. Em algumas conversas, pode parecer que você está falando sobre algo místico, mas esses são apenas documentos mundanos. A realidade é que uma boa estratégia de engenharia é entediante e é mais fácil escrever uma estratégia eficaz do que uma ruim.

Para escrever uma estratégia de engenharia, escreva cinco documentos de design e destaque as semelhanças. Isso é a sua estratégia de engenharia. Para escrever uma visão de engenharia, escreva cinco estratégias de engenharia e preveja suas implicações para daqui a dois anos. Isso é a sua visão de engenharia.

Se você não conseguir resistir à vontade de incluir suas ideias mais brilhantes no processo, pode incluí-las no seu trabalho preliminar. Escreva todas as suas melhores ideias em um documento gigante, delete-o e nunca mais mencione nenhuma delas. Agora que essas ideias estão fora da sua cabeça, sua mente está livre para o trabalho que vem a seguir.

Estratégia de engenharia e visão duradouramente úteis são o resultado da aprendizagem organizacional iterativa de baixo para cima. Como tal, toda aprendizagem contribui para a estratégia e visão de sua organização, mas sua contribuição não precisa ser tão abstrata. Mesmo que você não seja diretamente responsável por esse trabalho, existem etapas práticas que **você** pode tomar para avançar na estratégia e visão de sua organização, começando **agora mesmo**.

## Quando e por que

Antes de mergulhar na receita para criar estratégias e visões eficazes,
uma boa pergunta inicial é: "Quando e por que devo realmente criá-las?"
Estratégias são ferramentas de alinhamento proativo que capacitam equipes a avançar rapidamente e com confiança.
As estratégias permitem que todos - não apenas alguns privilegiados - tomem decisões rápidas e confiantes que, de outra forma, poderiam custar uma semana de discussão.
As estratégias também são os blocos de construção que reduzem suas muitas futuras possibilidades o suficiente para que seja possível escrever uma visão realista.
Se você perceber que reiterou a mesma discussão três ou quatro vezes, é hora de escrever uma estratégia.
Quando o futuro está muito incerto para identificar investimentos que valem a pena, é hora de escrever outra visão.
Se nenhum desses problemas parece familiar - siga em frente para outro trabalho por enquanto e volte mais tarde.

## Escreva cinco documentos de design

Documentos de design descrevem as decisões e compensações que você fez em projetos específicos. Sua empresa pode chamá-los de RFCs ou especificações técnicas. Nomes estranhos também acontecem; a Uber os chamava estranhamente de DUCKS até que posteriormente [padronizou em RFC](https://blog.pragmaticengineer.com/scaling-engineering-teams-via-writing-things-down-rfcs/). Um bom documento de design descreve um problema específico, analisa possíveis soluções e explica os detalhes da abordagem selecionada. Existem muitos formatos para escolher; alguns lugares para começar a pensar são [Design Docs, Markdown e Git](https://caitiem20.wordpress.com/2020/03/29/design-docs-markdown-and-git/), [Design Docs na Google](https://www.industrialempathy.com/posts/design-docs-at-google/) e [Tomada de Decisão Técnica e Alinhamento em uma Cultura Remota](https://multithreaded.stitchfix.com/blog/2020/12/07/remote-decision-making/).

Se um determinado projeto requer ou não um documento de design depende do julgamento pessoal, mas encontrei algumas regras úteis. Você deve escrever documentos de design para qualquer projeto cujas capacidades serão usadas por inúmeros projetos futuros. Você também deve escrever documentos de design para projetos que impactam significativamente seus usuários. Você deve escrever um documento de design para qualquer trabalho que leve mais de um mês de tempo de engenharia.

Um lote de cinco documentos de design é o ingrediente ideal para escrever uma estratégia eficaz, porque os documentos de design têm o que as más estratégias não têm: detalhes específicos ancorados na realidade. É fácil para dois engenheiros bem-intencionados na mesma equipe interpretar uma estratégia abstrata de maneiras diferentes, mas é muito mais difícil permanecer desalinhado quando você está implementando uma solução específica.


## Algumas recomendações ao escrever:

- **Comece pelo problema.** Quanto mais clara for a declaração do problema, mais óbvias serão as soluções. Se as soluções não forem óbvias, gaste mais tempo esclarecendo o problema. Se você estiver com dificuldades para articular o problema, mostre o que você tem para cinco pessoas e pergunte o que está faltando: olhos frescos sempre enxergam a verdade.

- **Mantenha o modelo simples.** A maioria das empresas possui um modelo de documento de design, que é um ótimo padrão a seguir. No entanto, esses modelos muitas vezes são expandidos para atender a muitos objetivos. Modelos sobrecarregados desencorajam as pessoas de escrever documentos de design em primeiro lugar. Prefira modelos de documentos de design mínimos que permitam aos autores selecionar as seções mais úteis e exijam detalhes exhaustivos apenas para os projetos mais arriscados.

- **Reúna e reveja juntos, escreva sozinho.** É muito improvável que você pessoalmente tenha todo o contexto relevante para escrever o melhor documento de design sobre um determinado tópico. Antes de entrar profundamente no processo, colete informações de pessoas com perspectivas relevantes, especialmente aquelas que dependerão do resultado do seu documento de design. No entanto, seja cético em relação ao processo colaborativo de escrita do documento de design em si. A maioria das pessoas é melhor escritora do que editora. Isso significa que geralmente é mais difícil editar um documento de grupo em escrita clara do que identificar um autor para escrever um documento claro. Reúna perspectivas amplamente, mas escreva sozinho. Apenas tenha cuidado para não se apaixonar pelo que você escreveu até <em>depois</em> de revisá-lo com outras pessoas.

- **Prefira o bom ao perfeito.** É melhor escrever um bom documento e colocá-lo na frente de outras pessoas do que adiar por algo marginalmente melhor. Isso é especialmente valioso para se ter em mente ao dar feedback sobre os designs de outras pessoas; é fácil cair na armadilha de esperar que seus designs sejam tão bons quanto o seu melhor design. Especialmente à medida que você avança em sua carreira, é prejudicial empurrar todos os designs para atender ao padrão do seu melhor trabalho. Concentre-se em fazer com que os designs sejam bons, em vez de fixar-se em seu próprio melhor como o padrão relevante de qualidade.

> **Leva muita prática para escrever ótimos documentos de design. Se você deseja melhorar os seus, meu melhor conselho é reler os seus designs <em>depois</em> de terminar de implementá-los e estudar os lugares onde a sua implementação se desviou do seu plano - o que causou essas divergências? Ah, e claro, continue escrevendo mais deles.**

## Sintetize esses cinco documentos de design em uma estratégia

Após sua organização ter escrito cinco documentos de design, sente-se e leia todos eles juntos. Procure por decisões controversas que surgiram em vários designs, especialmente aquelas que foram difíceis de concordar. Um exemplo recente meu foi ficar preso debatendo se o Redis era apropriado como armazenamento durável ou apenas como cache. Em vez de começar do zero em cada revisão do documento de design, não seria mais fácil se revisássemos nossas decisões recentes sobre o uso do Redis, refletíssemos sobre como tomamos essas decisões e as escrevêssemos como uma estratégia?

Boas estratégias orientam as compensações e explicam o raciocínio por trás desse direcionamento. Estratégias ruins estabelecem uma política sem explicação, o que as desconecta do contexto em que foram tomadas. Sem contexto, sua estratégia rapidamente se torna incompreensível - por que eles decidiram isso? - e difícil de adaptar à medida que o contexto subjacente muda. Alguns estratégias interessantes para ler enquanto pensa em escrever a sua própria estão em [A Framework for Responsible Innovation](https://multithreaded.stitchfix.com/blog/2019/08/19/framework-for-responsible-innovation/) e [How Big Technical Changes Happen at Slack](https://slack.engineering/how-big-technical-changes-happen-at-slack/).

Se você é um convertido do livro [Good Strategy, Bad Strategy](https://www.amazon.com/dp/B004J4WKEC) - e esse livro transformou completamente minha maneira de pensar sobre estratégia - então você notará que essa definição de estratégia é "diagnóstico" e "políticas orientadoras", adiando "ação coerente" para os documentos de design.

## Minhas melhores dicas para escrever um documento de estratégia são:

- **Comece de onde você está.** Ao trabalhar em estratégia, é fácil ser paralisado pela vasta ambiguidade com a qual trabalhamos, mas você só precisa mergulhar e começar a escrever. Esperar por informações que estão faltando não funciona: cada documento ausente está ausente por um bom motivo. O que quer que você escreva precisará mudar, e se você escrever algo especialmente ruim, perceberá rapidamente a necessidade de mudá-lo. Onde você está agora é sempre o melhor lugar para começar.

- **Escreva os detalhes.** Escreva até começar a generalizar e, em seguida, pare de escrever. Se você não pode ser específico, espere até ter escrito mais documentos de design. Declarações específicas criam alinhamento; declarações genéricas criam a ilusão de alinhamento.

- **Seja opinativo.** Boas estratégias são opinativas. Se não forem opinativas, não fornecerão clareza na tomada de decisões. No entanto, ser opinativo por si só não é suficiente. Você também precisa mostrar o seu trabalho.

- **Mostre o seu trabalho.** Nas aulas de matemática quando crianças, tínhamos que mostrar o nosso trabalho para obter nota máxima. Aqui também, você deve mostrar o raciocínio por trás das suas opiniões. Mostrar o seu trabalho cria confiança na primeira versão de um documento, mas, mais importante ainda, ao mostrar o seu trabalho, você torna possível para outras pessoas modificarem e ampliarem o seu trabalho à medida que o contexto subjacente muda.

> **Algumas das melhores estratégias que você escreverá podem, na época, parecer muito óbvias para se preocupar em escrever. "Quando devemos escrever documentos de design?" é uma estratégia que vale a pena escrever. "Quais bancos de dados usamos para quais casos de uso?" é uma estratégia que vale a pena escrever. "Como devemos planejar nossa migração do monólito para serviços?" também vale a pena escrever. À medida que deixamos para trás a ideia de estratégia como demonstrações de brilhantismo, podemos começar a escrever muito mais delas e podemos escrevê-las de maneira mais informal. Se ela acabar não sendo usada, você sempre pode descontinuá-la posteriormente.

## Extrapole cinco estratégias em uma visão

À medida que você coleta mais estratégias, se tornará cada vez mais desafiador raciocinar sobre como as várias estratégias interagem. Talvez uma das suas estratégias seja <a href="https://www.intercom.com/blog/run-less-software/">Rodar menos software</a> e confiar mais em soluções em nuvem, mas outra das suas estratégias seja preferir a transferência de complexidade para o banco de dados sempre que possível. Como você concilia essas estratégias se identificar um banco de dados que permitiria transferir uma grande quantidade de complexidade, mas que não é oferecido pelo seu fornecedor de nuvem?

Pegue cinco de suas estratégias recentes, extrapole como suas compensações se desenrolarão nos próximos dois a três anos. Conforme você edita as contradições e entrelaça os fios, você escreveu uma visão de engenharia. A versão final lhe dará o que [Tanya Reilly](https://twitter.com/whereistanya) chama de [uma crença robusta no futuro](https://leaddev.com/technical-direction-strategy/sending-gifts-future-you), o que facilita entender como suas estratégias existentes se relacionam umas com as outras e simplifica a escrita de novas estratégias que resistem ao teste do tempo.

Para uma visão útil, foque em algumas coisas:

- **Escreva daqui a dois a três anos.** Empresas, organizações e tecnologia mudam rapidamente demais para pensar muito no futuro. Também não funciona se você escrever uma visão que expira em seis meses - quantas estratégias você escreveria realisticamente dentro desse prazo de seis meses? Tente focar daqui a dois a três anos; você pode expandir esse horizonte um pouco se for uma empresa já estabelecida.

- **Baseie-se no seu negócio e nos seus usuários.** VIsões eficazes se baseiam em servir seus usuários e seu negócio. Essa conexão estreita mantém a visão alinhada com os valores centrais da sua equipe de liderança - usuários e negócios. Visões ruins tratam a sofisticação técnica como uma razão de ser autojustificada - uma visão que nunca é compartilhada pela liderança da sua empresa.

-