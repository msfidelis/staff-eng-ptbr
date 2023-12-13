---
title: Operando como Staff / Gerencie a Qualidade Tecnica
author: Tao He
date: 2023-12-08
category: OperatingAtStaff
layout: post
mermaid: true
---

> Sinto-me especialmente impactante quando posso ajudar a melhorar uma proposta bem-intencionada que resolve uma necessidade real, mas a equipe que a redigiu carece de experiência ou contexto para criar um bom plano para capturar a oportunidade. Em tais casos, ter um plano bem estruturado pode ajudar substancialmente a reduzir o escopo enquanto se chega à maior parte do valor, e assim demonstrar impacto mais cedo.
> \- [Dmitry Petrashko](/stories/dmitry-petrashko)

Se há algo com que engenheiros, gerentes de engenharia e executivos de tecnologia provavelmente concordarão, é que há uma crise de qualidade técnica. Um diagnóstico e uma cura são fáceis de identificar: nossos engenheiros não estão priorizando a qualidade e precisamos contratar engenheiros melhores ou requalificar os que temos. Claro, sinta-se à vontade para substituir "engenheiros" por "gerentes de produto" ou "executivos" se isso parecer mais confortável. É uma narrativa cativante com um vilão claro e convenientemente desloca a culpa da liderança de engenharia. No entanto, assim como a maioria das narrativas que transferem a responsabilidade para as pessoas com menos poder, ela é tanto inútil quanto errada.

Quando você aceita a premissa de que a baixa qualidade técnica resulta de decisões ruins, começa a procurar por julgamentos ruins, e alguém na empresa deve ser o culpado. É o CTO anterior? É aquele engenheiro sênior olhando para você com um sorriso nervoso? É todo mundo? E se não forem essas pessoas, e ainda mais estranho, não é culpa sua também?

Na maioria dos casos, a baixa qualidade técnica não é uma crise; é o estado normal esperado. Os engenheiros geralmente tomam decisões razoáveis de qualidade quando as tomam, e as empresas bem-sucedidas elevam sua barra de qualidade ao longo do tempo, à medida que crescem, fazem pivôs ou se voltam para o mercado empresarial. Em uma empresa bem administrada e bem-sucedida, a maioria das decisões técnicas anteriores não atenderá ao seu padrão de qualidade atual. Em vez de um fracasso, fechar a lacuna entre sua qualidade técnica atual e alvo é uma parte rotineira e essencial da liderança de engenharia eficaz.

<br>

## O problema

Como equipe de liderança de engenharia, seu objetivo é manter um nível de qualidade técnica apropriado enquanto dedica o máximo de energia possível ao negócio principal. Você precisa equilibrar a qualidade em vários horizontes temporais, e esses horizontes geralmente têm necessidades conflitantes. Por exemplo, você fará um trabalho muito diferente para lançar aquela parceria crítica na próxima semana em comparação com a construção de uma plataforma que suporte lançamentos dez vezes mais rápidos no próximo trimestre.

Assim como a barra de qualidade técnica de sua empresa mudará ao longo do tempo, sua abordagem para gerenciar a qualidade técnica evoluirá em conjunto:

1. corrija os **pontos críticos** que estão causando problemas imediatos
2. adote as **melhores práticas** conhecidas por melhorar a qualidade
3. priorize os **pontos de alavancagem** que preservam a qualidade à medida que seu software muda
4. alinhe os **vetores técnicos** na forma como sua organização altera o software
5. **meça a qualidade técnica** para orientar investimentos mais profundos
6. inicie uma **equipe de qualidade técnica** para criar sistemas e ferramentas para qualidade
7. execute um **programa de qualidade** para medir, rastrear e criar responsabilidade

Conforme exploramos este conjunto de abordagens, lembre-se de escolher a ferramenta mais barata e direta que provavelmente funcionará. A qualidade técnica é um jogo de longo prazo. Não há como vencer, apenas aprender e ganhar a chance de continuar jogando.

<br>

## Ascendendo a escada

Existe uma alegria particular em aprofundar o desafio em questão até encontrar um problema generalizado que vale a pena resolver. No entanto, um instinto igualmente importante é resolver rapidamente a situação atual e avançar para o próximo problema urgente.

Ao pensar nas melhorias de qualidade certas para sua equipe e organização, geralmente é mais eficaz começar com soluções mais leves e progredir apenas para soluções maciças à medida que os esforços anteriores desmoronam sob a pressão da escala. Se você não conseguir fazer com que as equipes adotem a formatação de código adequada, seus esforços para implementar um programa de qualidade abrangente estão condenados. Embora este último possa ser mais eficaz em grande escala, é muito, muito mais difícil de executar.

Então, faça primeiro as coisas rápidas!

Mesmo que não funcione, você aprenderá mais rapidamente a partir do fracasso em implementar o fácil do que em implementar o difícil. Com o tempo, você avançará em direção a abordagens abrangentes, mas não há necessidade de pressa. Não abandone a facilidade, a alegria e a inocência das organizações iniciais pelos perigos da coordenação em escala empresarial sem a necessidade adequada.

É conveniente apresentar essas fases como uma escada linear a ser ascendida, mas raramente é assim que as organizações reais as usam. É mais provável que você corrija um ponto crítico de qualidade, implemente uma melhor prática, comece a realizar uma revisão de arquitetura, abandone essa revisão de arquitetura e volte a se concentrar nos pontos críticos por um tempo. Processos prematuros adicionam mais atrito do que valor e rapidamente se revelam ineficazes. Se algo não estiver funcionando, tente fazê-lo funcionar por um tempo e depois celebre o seu fim.

<br>

## Pontos críticos

Quando confrontados com um problema de qualidade, o primeiro instinto muitas vezes é identificar uma falha no processo que necessariamente requer uma solução de processo. Se uma implantação causa uma interrupção, é porque o autor não seguiu corretamente o processo de teste de código, então agora vamos exigir testes com cada commit - isso ensinará aqueles desenvolvedores preguiçosos!

Há a antiga piada sobre o Sarbanes-Oxley: ele não reduz o risco; apenas torna claro quem culpar quando as coisas dão errado. Infelizmente, essa piada se aplica sem humor a quantas organizações implementam processos. A responsabilidade tem seu papel, mas é muito mais importante entender o problema em questão e tentar corrigi-lo diretamente do que criar responsabilidade orientada por processo.

A implementação de processos requer que os seres humanos mudem a forma como trabalham, o que você não deve empreender levianamente. Em vez de buscar a melhoria de processos, comece adotando a mentalidade de engenheiro de desempenho. Meça o problema em questão, identifique onde ocorre a maior parte do problema e concentre-se precisamente nessa área.

O exemplo anterior de uma implantação não testada pode se beneficiar em dar um feedback direto ao engenheiro que está realizando a implantação sobre a mudança de seus hábitos de teste. Alternativamente, talvez você esteja melhor servido reconhecendo que seu design de software é propenso a erros e adotando a abordagem de "definir erros fora da existência" descrita em [A Philosophy of Software Design](https://www.amazon.com/Philosophy-Software-Design-John-Ousterhout/dp/1732102201).

Se você tiver um problema de velocidade de desenvolvimento, talvez seja otimizar os tempos de execução dos testes, mover sua etapa de compilação do Docker para um [disco RAM](https://en.wikipedia.org/wiki/RAM_drive) ou usar as técnicas descritas em [Software Design X-Rays](https://www.amazon.com/Software-Design-X-Rays-Technical-Behavioral-ebook-dp-B07BVRLZ87/dp/B07BVRLZ87/) para encontrar os arquivos específicos a serem melhorados.

A [pensamento sistêmico](https://lethain.com/systems-thinking/) é a técnica de pensamento mais transformadora que encontrei em minha carreira. Ainda assim, às vezes pode ser um canto de sereia que o atrai para corrigir um sistema atual que você pode estar melhor descartando. Claro, você pode implementar um novo programa de treinamento para ensinar sua equipe a escrever testes melhores, mas alternativamente, talvez você possa simplesmente excluir o arquivo de teste em que 98% das falhas ocorrem. Essa é a eficácia irracional de priorizar pontos críticos e por que isso deve ser a primeira técnica que você usa para melhorar a qualidade técnica.

Em algum momento, você provavelmente descobrirá que sua organização está criando problemas de qualidade mais rapidamente do que você consegue corrigir os pontos críticos, e é aí que é hora de passar para a adoção das melhores práticas.

## Melhores Práticas

Uma vez trabalhei em uma empresa que não tinha um processo de planejamento de equipe. Com o tempo, o chefe de engenharia ficou cada vez mais frustrado com a incapacidade de projetar datas-alvo e decretou que usaríamos o <a href="https://en.wikipedia.org/wiki/Scrum_(software_development)">Scrum</a>. Após o decreto, um gerente escreveu o processo Scrum em uma wiki. Houve um anúncio de que estávamos usando o Scrum. Os gerentes disseram às suas equipes para usar o Scrum. Missão cumprida!

Claro, ninguém começou a usar o Scrum. Todos continuaram fazendo o que faziam antes. É constrangedor reconhecer erros, então o chefe de engenharia declarou a adoção um grande sucesso, e ninguém teve coragem de discordar.

Essa triste história reflete como muitas empresas tentam implementar melhores práticas, e é uma das razões pelas quais as melhores práticas têm tão má reputação. Em teoria, as organizações se beneficiariam ao adotar melhores práticas antes de corrigir pontos críticos de qualidade, mas eu recomendo práticas após a identificação dos pontos críticos. A adoção de melhores práticas requer um nível de maturidade organizacional e de liderança que leva algum tempo para se desenvolver.

Quando você está implementando uma nova prática, lembre-se de que um <a href="https://lethain.com/good-process-is-evolved/">bom processo é evoluído</a> em vez de imposto. Estude como outras empresas adotam práticas semelhantes, documente sua abordagem pretendida, experimente a prática com algumas equipes envolvidas, aprimore os detalhes com base nos desafios encontrados e só então a expanda. Um processo apressado é um processo falido.

Tão importante quanto é a ideia de limitar a implementação simultânea de práticas. Se você tentar fazer com que as equipes adotem várias práticas novas simultaneamente, estará competindo por sua atenção consigo mesmo. Também torna mais difícil atribuir impacto posteriormente se estiver considerando reverter ou modificar uma das novas práticas. É um pouco draconiano, mas eu cheguei a acreditar que você deve se limitar a uma única implementação de melhores práticas a qualquer momento. Concentre toda a sua energia em fazer de uma prática um sucesso em vez de dividir recursos entre várias.

A adoção de uma única nova prática por vez também o força a pensar cuidadosamente sobre qual priorizar. Escolher seu próximo processo parece fácil, mas muitas vezes não está claro quais melhores práticas são verdadeiramente melhores práticas e quais são apenas familiares ou famosas. Uma melhor prática genuína deve ser respaldada por pesquisa, e a melhor fonte de pesquisa sobre esse tópico é <a href="https://www.amazon.com/dp/B07B9F83WM/">Accelerate</a>.

Embora todas as recomendações do Accelerate sejam baseadas em dados e bastante boas, as poucas que encontrei mais úteis para adotar inicialmente são o controle de versão, o desenvolvimento baseado em tronco, a CI/CD e a observabilidade em produção (incluindo desenvolvedores de plantão para os sistemas que escrevem) e o trabalho com mudanças pequenas e atômicas. Existem muitas outras práticas que eu adoraria defender (quem não passou uma era de carreira defendendo <a href="https://increment.com/documentation/why-investing-in-internal-docs-is-worth-it/">documentação interna melhor</a>), mas eu não confio mais na minha intuição como costumava fazer.

A transição da correção de pontos críticos para a adoção de melhores práticas acontece quando você está sobrecarregado por muitos pontos críticos para resolver. A próxima transição, das melhores práticas para pontos de alavancagem, acontece quando você se vê querendo adotar uma nova melhor prática antes que sua melhor prática em andamento esteja funcionando. Em vez de <a href="https://lethain.com/limiting-wip/">aumentar seu limite de adoção de melhores práticas em andamento</a>, siga para a próxima ferramenta.

## Pontos de Alavancagem

Na seção anterior sobre Pontos Críticos, falamos sobre usar a mentalidade de engenheiro de desempenho para identificar os problemas certos a serem resolvidos. A otimização funciona bem para os problemas que você já tem, mas é intencionalmente inaplicável ao futuro: o pior pecado do engenheiro de desempenho é aplicar esforço a problemas não comprovados.

No entanto, ao analisar como o software muda ao longo do tempo, existem algumas poucas áreas onde investimento adicional preserva a qualidade ao longo do tempo, tanto ao evitar falhas graves de qualidade quanto ao reduzir o custo de investimentos futuros em qualidade.

Eu chamo esses pontos de alavancagem de qualidade, e os três mais impactantes são interfaces, sistemas com estado e modelos de dados.

<em>Interfaces</em> são contratos entre sistemas. Interfaces eficazes desacoplam os clientes da implementação encapsulada. Interfaces duráveis expõem toda a complexidade essencial subjacente e nenhuma da complexidade acidental subjacente. Interfaces agradáveis são <a href="https://increment.com/apis/api-design-for-eager-discering-developers/">Discernidamente ansiosas, discernidamente ansiosas</a>.

<em>Estado</em> é a parte mais difícil de qualquer sistema de se alterar, e essa resistência à mudança torna <em>sistemas com estado</em> outro ponto de alavancagem crítico. O estado fica complexo mais rapidamente do que outros sistemas e tem uma inércia que o torna relativamente caro de melhorar posteriormente. À medida que você incorpora obrigações comerciais relacionadas à segurança, privacidade e conformidade, a mudança em seus sistemas com estado se torna ainda mais desafiadora.

<em>Modelos de dados</em> são a interseção das interfaces e do estado, restringindo as capacidades de seus sistemas com estado ao que sua aplicação considera legal. Um bom modelo de dados é rígido: ele apenas expõe o que realmente suporta e impede a expressão de estados inválidos. Um bom modelo de dados é tolerante à evolução ao longo do tempo. Modelos de dados eficazes não são nem um pouco inteligentes.

Conforme você identifica esses pontos de alavancagem em seu trabalho, dedique tempo extra para abordá-los deliberadamente. Se for uma interface, integre meia dúzia de clientes na implementação simulada. Se for um modelo de dados, represente meia dúzia de cenários reais. Se for com estado, simule os modos de falha, verifique os comportamentos de consistência e estabeleça benchmarks de desempenho semelhantes ao seu cenário de produção.

Leve tudo o que você aprendeu e coloque-o em um documento de especificação técnica que você compartilhe com sua equipe. Colete feedback do setor entre seus pares. Mesmo depois de começar a implementação, ouça a voz da realidade e mantenha-se aberto a mudanças.

Um dos poderes ocultos de investir em pontos de alavancagem é que você não precisa de um alinhamento organizacional total para fazê-lo. Para escrever uma visão técnica ou implementar uma melhor prática, você precisa desse tipo de comprometimento, por isso recomendo começar com pontos de alavancagem. No entanto, se você esgotou o impacto acessível dos pontos de alavancagem, pode ser hora de passar para a condução de um alinhamento organizacional mais amplo.

## Vetores Técnicos

Organizações eficazes direcionam a maioria de seus esforços para uma visão compartilhada. Se você representar cada decisão técnica como um vetor em um plano, quanto mais esses vetores apontarem na mesma direção, mais você alcançará ao longo do tempo. Por outro lado, alguns dos engenheiros mais impressionantes com quem trabalhei criaram vetores com uma magnitude extraordinária, mas uma direção desalinhada. 
No final, esses engenheiros prejudicaram suas organizações em suas tentativas de liderá-las.

Uma solução infalível para alinhar a direção técnica é rotear todas as decisões relacionadas para a mesma pessoa com <a href="https://staffeng.com/guides/staff-archetypes">Arquiteto</a> em seu título. Isso funciona bem, mas é desafiador de escalar, e a qualidade das decisões de um arquiteto degrada quanto mais longe eles ficam do trabalho real em código real no processo real. No outro extremo, você pode permitir que cada equipe tome decisões independentes. Mas uma organização que permite qualquer ferramenta é uma organização com ferramentas uniformemente não suportadas.

Suas ferramentas fundamentais para alinhar vetores técnicos são:

- **Dê feedback direto.** Quando as pessoas se deparam com desalinhamentos, a primeira resposta geralmente é mudança de processo, mas, em vez disso, comece dando feedback direto às pessoas que você acredita estarem desalinhadas. Assim como eles estão perdendo o seu contexto, você está perdendo o deles, e uma conversa rápida muitas vezes pode evitar anos de processo desnecessário.

- **Refine sua estratégia de engenharia** de <a href="/guides/engineering-strategy">especificação técnica, estratégia, visão</a>.

- **Incorpore sua abordagem em seus fluxos de trabalho e ferramentas.** A documentação de uma visão clara é útil, mas algumas pessoas simplesmente não estudarão seu documento. Ferramentas deliberadas criam fluxos de trabalho que incentivam hábitos muito melhor do que treinamento e documentação. Por exemplo, a provisionamento de um novo serviço pode exigir que você vá a um site que o obriga a adicionar um link para uma especificação técnica desse serviço. Outra abordagem pode ser bloquear as implantações em produção se o serviço não tiver uma configuração de plantão estabelecida, com alguém atualmente de plantão, e essa pessoa também deve ter suas notificações push habilitadas.

- **Treine novos membros da equipe durante o processo de integração.** Mudar os hábitos das pessoas depois que eles já se formaram é bastante desafiador, o que é frustrante se você estiver tentando fazer as pessoas adotarem novas práticas. No entanto, se você direcionar as pessoas na direção certa quando elas entrarem, o ímpeto do hábito funcionará a favor do alinhamento.

- **Use a <em>Lei de Conway</em>.** A Lei de Conway argumenta que as organizações constroem software que reflete sua estrutura. Se sua organização for mal estruturada, isso levará a software fortemente acoplado ou emaranhado. No entanto, também é uma força para a qualidade se o design de sua organização for eficaz.

- **Crie mudanças de tecnologia com curadoria** usando <a href="https://lethain.com/scaling-consistency/">análises de arquitetura</a>, <a href="https://lethain.com/magnitudes-of-exploration/">estratégias de investimento</a> e <a href="https://slack.engineering/how-big-technical-changes-happen-at-slack/">um processo estruturado para adotar novas ferramentas</a>. A maioria dos desalinhamentos ocorre pela falta de contexto, e esses são os pontos de alavancagem organizacional para injetar contexto na tomada de decisões. Muitas organizações começam por aqui, mas é a última caixa de ferramentas que recomendo abrir. Como você pode fornecer análises de arquitetura consistentes sem uma visão articulada? Por que dizer às pessoas sua estratégia depois que elas já projetaram algo em vez de durante o processo de integração delas?

Independentemente das abordagens que você usa para alinhar seus vetores técnicos, este é um trabalho que tende a ocorrer ao longo de meses e anos. Não há um mundo onde você escreva o documento de visão e a organização imediatamente se alinha atrás de sua genialidade. Muito mais provável é que ele acumule poeira até que você invista na construção de apoio.

A maioria das empresas pode combinar as técnicas acima, desde a correção de pontos críticos até o alinhamento de vetores, em uma abordagem bem-sucedida para gerenciar a qualidade técnica, e espero que seja o caso para você. No entanto, muitas descobrem que não são suficientes e que você passa para abordagens mais pesadas. Nesse caso, o primeiro passo é, como sempre, a medição.

## Medir a qualidade técnica

O desejo de medir na engenharia de software geralmente supera nosso estado de medição. <a href="https://www.amazon.com/dp/B07B9F83WM/">Accelerate</a> identifica métricas para medir a velocidade, que são poderosas para identificar problemas de processo e ferramentas, mas essas métricas começam <em>após</em> o código ter sido mesclado. Como medir a qualidade do seu código-fonte de forma que você possa identificar lacunas, propor um plano de ação e avaliar o impacto de seus esforços para melhorar?

Existem algumas medidas de processo que se correlacionam com mudanças eficazes. Por exemplo, você pode medir o número de arquivos alterados em cada solicitação pull, com a compreensão de que solicitações pull menores geralmente têm uma qualidade mais alta. Você também pode medir o número de linhas de código por arquivo em um código-fonte, sob a suposição de que arquivos muito grandes geralmente são difíceis de estender. Essas medidas podem ser bastante úteis, e eu até recomendaria medi-las, mas acredito que elas são, na melhor das hipóteses, medidas proxy para qualidade de código.

Minha experiência é que é <em>possível</em> medir de forma útil a qualidade do código e isso se resume a desenvolver uma definição extremamente precisa de qualidade. Quanto mais detalhada for a sua definição de qualidade, mais útil ela se torna para medir um código-fonte e mais instrutiva ela se torna para as pessoas que esperam melhorar a qualidade da área em que estão trabalhando. Essa abordagem é descrita em detalhes em <a href="https://www.amazon.com/Building-Evolutionary-Architectures-Support-Constant/dp/1491986360/">Building Evolutionary Architectures</a> e <a href="https://lethain.com/reclaim-unreasonable-software/">Reclaim unreasonable software</a>.

Alguns componentes representativos a serem considerados em sua definição de qualidade:

- Qual a porcentagem do código é tipada estaticamente?
- Quantos arquivos têm testes associados?
- Qual é a cobertura de testes em seu código-fonte?
- Quão estreitas são as interfaces públicas entre módulos?
- Qual a porcentagem de arquivos usa a biblioteca HTTP preferida?
- Os pontos finais respondem às solicitações em menos de 500ms após uma inicialização a frio?
- Quantas funções têm um comportamento perigoso de leitura após gravação? Ou realizam leituras desnecessárias na instância de banco de dados primária?
- Quantos pontos finais realizam todas as mutações de estado dentro de uma única transação?
- Quantas funções adquirem travas de baixa granularidade?
- Quantos arquivos quentes existem que são alterados em mais da metade das solicitações pull?

Você pode discordar que algumas dessas propriedades devem existir na definição de qualidade do <em>seu</em> código-fonte: sua definição deve ser específica para o seu código e suas necessidades. O importante é desenvolver uma definição precisa e mensurável. Haverá discordância no desenvolvimento dessa definição, e você inevitavelmente mudará a definição ao longo do tempo.

Após desenvolver a definição, esta é uma área em que a instrumentação pode ser genuinamente desafiadora, e a instrumentação é um requisito para métricas úteis. A complexidade da instrumentação é o maior ponto de atrito para a adoção dessas técnicas na prática, mas se você conseguir superá-la, desbloqueará algo bastante fenomenal: uma pontuação de qualidade real e dinâmica que você pode acompanhar ao longo do tempo e usar para criar uma clareza de alinhamento em sua abordagem que o alinhamento conceitual não pode proporcionar.

Com a qualidade definida e instrumentada, seu próximo passo é decidir entre investir em uma <em>equipe de qualidade</em> ou um <em>programa de qualidade</em>. Uma equipe dedicada é fácil de coordenar e previsível em sua capacidade e geralmente é o lugar mais fácil para começar.

## Equipe de Qualidade Técnica

Uma <em>equipe de qualidade técnica</em> é uma equipe de engenharia de software dedicada a criar qualidade em seu código-fonte. Você pode chamar essa equipe de Produtividade do Desenvolvedor, Ferramentas do Desenvolvedor ou Infraestrutura de Produto. Em qualquer caso, o objetivo da equipe é criar e preservar a qualidade em todo o software da sua empresa.

Isso não é o que às vezes é chamado de equipe de garantia de qualidade. Embora ambas as equipes façam investimentos em testes, a equipe de qualidade técnica tem um escopo mais amplo, desde o fluxo de trabalho até a construção, os testes e o design da interface.

Ao iniciar uma equipe dessas, comece com um tamanho fixo de equipe de três a seis pessoas. Ter uma equipe pequena o força a priorizar implacavelmente o roteiro com base no impacto e garante que você mantenha o foco no que é alcançável. Com o tempo, essa equipe acumulará sistemas que exigem investimento em escala, clusters Jenkins são um exemplo comum disso, e você desejará <a href="https://lethain.com/sizing-engineering-teams/">dimensionar a equipe</a> como uma função da organização de engenharia mais ampla. As regras práticas são complicadas aqui, mas talvez um engenheiro trabalhando em ferramentas para desenvolvedores para cada quinze engenheiros de produto, além do seu investimento em engenharia de infraestrutura.

É raro que essas equipes tenham um gerente de produtos. Geralmente, há um ou mais engenheiros do nível "Staff" ou superior e o parceiro gerente de engenharia que desempenha esse papel. Às vezes, eles empregam um Gerente de Programa Técnico, mas normalmente isso ocorre depois que eles entram em operação em um <em>programa de qualidade</em>, conforme descrito na próxima seção.

Ao criar e operar uma dessas equipes, alguns fundamentos para o sucesso são:

1. **Confie em métricas em vez de intuição.** Você deve ter uma maneira de medir cada projeto. A qualidade é um sistema complexo, o tipo de lugar onde sua intuição pode facilmente enganá-lo. Da mesma forma, à medida que você avança na hierarquia de sua empresa, sua experiência não refletirá mais as experiências da maioria das outras pessoas. Você já conhece os pontos fracos e será a primeira pessoa a receber ajuda se encontrar um novo, mas a maioria das outras pessoas não. As métricas mantêm você honesto.

2. **Mantenha sua intuição atualizada.** O código e o processo mudam ao longo do tempo, e sua intuição fica obsoleta a cada semana que você está longe de criar recursos de produto. A maioria das pessoas descobre que a incorporação de equipe e as rotações de equipe são a melhor maneira de manter seus instintos relevantes. Outros monitoram bate-papos em busca de problemas, além de uma agenda saudável de discussões individuais com desenvolvedores de produtos. Os melhores fazem ambas as coisas e mantêm seus painéis de métricas à mão.

3. **Ouça e aprenda com seus usuários.** Existe uma ideia popular de "nível de gosto", que implica que algumas pessoas simplesmente sabem como é algo bom. Existe uma grande variabilidade nas pessoas que projetam investimentos em qualidade eficazes, mas não é uma habilidade inata. As melhores pessoas se concentram em entender profundamente o que seus usuários estão tentando realizar e priorizam as necessidades do usuário sobre as restrições de implementação.

4. **Faça menos coisas, mas faça-as melhor.** Quando você está construindo para toda a organização de engenharia, qualquer coisa que você faça bem acelerará a organização como um todo. Qualquer coisa que você faça mal, incluindo algo quase ótimo com muitas arestas ásperas, arrastará todos para baixo. Embora seja quase sempre verdade que fazer as poucas coisas mais importantes contribuirá mais do que muitos projetos medianos, isso é ainda mais verdadeiro nos casos em que você está tentando implantar ferramentas e fluxos de trabalho para toda a organização (os limites do processo em andamento da organização ainda se aplicam aqui!).

5. **Não guarde impacto para si mesmo.** Existe uma tensão fundamental entre equipes de qualidade centralizadas e as equipes que elas apoiam. É frequentemente o caso que existe uma abordagem globalmente ideal preferida pela equipe centralizada, que gera atrito em um subconjunto de equipes que trabalham em domínios ou cargas de trabalho atípicas. Um exemplo representativo é uma empresa que escreve seus servidores back-end em JavaScript e não permite que seus engenheiros de aprendizado de máquina usem o ecossistema Python porque não desejam suportar dois ecossistemas. Outro caso é uma empresa que padroniza o uso de REST/HTTP2/JSON para todas as APIs, onde uma equipe específica deseja usar gRPC em vez disso. Não há uma resposta perfeita aqui, mas é importante estabelecer uma abordagem ponderada que <a href="http://lethain.com/magnitudes-of-exploration/">equilibre os benefícios da exploração com os benefícios da padronização</a>.

Uma equipe de qualidade técnica bem-sucedida, usando as abordagens acima, será <em>indiscutivelmente</em> mais produtiva do que se o mesmo número de engenheiros estivesse fazendo diretamente o trabalho de engenharia de produto. Na verdade, a produtividade do desenvolvedor descontada (no espírito do <a href="https://en.wikipedia.org/wiki/Discounted_cash_flow">fluxo de caixa descontado</a>) é a maneira teoricamente correta de medir o impacto de tal equipe. Apenas teoricamente, porque tais cálculos são principalmente uma avaliação da sua autoconfiança.

Mesmo que você seja bastante bem-sucedido, sempre terá um backlog de trabalho de alto impacto que deseja assumir, mas não tem a capacidade de concluir. As organizações não tomam decisões de dimensionamento de equipe puramente racionais, e você pode descobrir que falta capacidade para concluir projetos importantes e, da mesma forma, não consegue aprovação para contratar mais pessoas para a sua equipe.

É um bom sinal quando sua equipe tem mais trabalho de alto impacto disponível do que você pode assumir: se você não for seletivo sobre quais projetos assumir, significa que você não está pensando amplamente o suficiente. Isso significa que você não deve necessariamente tentar expandir sua equipe de qualidade técnica se tiver um backlog. No entanto, se você descobrir que há trabalho crítico de qualidade que você não consegue realizar, pode ser hora de explorar a criação de um <em>programa de qualidade</em>.

## Programa de Qualidade

Um <em>programa de qualidade</em> não é código de computador, mas sim uma iniciativa liderada por uma equipe dedicada para manter a qualidade técnica em toda uma organização. Um programa de qualidade assume o amplo objetivo de atingir o nível de qualidade de software desejado pela organização. Esses programas são relativamente incomuns, mas algo semelhante que você provavelmente encontrou é um programa de incidentes responsável pelas retrospectivas de incidentes e pelas correções de uma empresa.

Os componentes técnicos de executar um programa de qualidade são semelhantes ao que foi discutido anteriormente. Portanto, aqui nos concentraremos em gerenciar um programa de forma eficaz. Seu primeiro passo é encontrar um gerente de programa técnico que possa co-liderar o programa e operar seus mecanismos. Embora você possa fazer um progresso considerável nos aspectos informativos de um programa organizacional sem um gerente de programa técnico, isso é um erro. Você será sobrecarregado pela sobrecarga de coordenação ao tentar liderar sozinho um programa em uma grande organização.

Operar programas organizacionais é <a href="https://lethain.com/programs-owning-the-unownable/">um tópico amplo sobre o qual muito já foi escrito</a>, mas a abordagem principal é a seguinte:

1. **Identifique um patrocinador do programa.** Você não pode mudar o comportamento de uma organização sem um patrocinador empoderado. As organizações se comportam da maneira que fazem porque é a solução ideal para as restrições atuais delas, e você não pode mudar essas restrições sem o apoio de alguém com poder.

2. **Gere métricas sustentáveis e reproduzíveis.** É comum que as pessoas que administram um programa gastem mais de quatro horas por semana mantendo seus dados manualmente. Isso não funciona. Seus dados terão lacunas, você não conseguirá integrar seus dados com automação nas etapas posteriores e você ficará sem energia para fazer o trabalho para efetuar uma mudança real; atualizar um painel de métricas não tem valor inerente.

3. **Identifique objetivos do programa para cada equipe impactada e um caminho claro para que eles alcancem esses objetivos.** Seu programa deve identificar metas específicas para cada equipe impactada. Por exemplo, reduzir a flutuação de testes em seus testes ou fechar correções de incidentes mais rapidamente. No entanto, é essencial fornecer o mapa para o sucesso! Muitos programas exigem a participação de outras equipes sem fornecer direções claras sobre como elas podem realizar sua parte. O proprietário do programa é o especialista no assunto, não transfira sua estratégia para cada equipe reinventar independentemente.

4. **Crie as ferramentas e documentação para apoiar as equipes em direção aos seus objetivos.** Depois de identificar um caminho claro para as equipes alcançarem os objetivos do seu programa, descubra como você pode ajudá-las a fazer essas mudanças! Isso pode incluir fornecer "exemplos de ouro" do que as coisas devem parecer, ou um pull request de exemplo que refatora uma seção desafiadora de código para o novo padrão. Pode ser fornecer um script de teste para verificar se a migração funcionou corretamente. Pode ser a geração automática do commit de conversão para testar, verificar e mesclar sem que os engenheiros o escrevam. Faça o máximo possível para evitar que cada equipe precise entender profundamente o espaço do problema que você está tentando avançar.

5. **Crie um painel de metas e compartilhe-o amplamente.** Depois de comunicar as metas do programa para cada equipe, forneça painéis que as ajudem a entender seu estado atual, seu estado desejado e que forneçam feedback reforçador sobre seu (esperançoso) progresso ao longo do caminho. O melhor painel será um placar para o trabalho de cada equipe e também fornecerá pistas para cada equipe sobre onde focar seus próximos esforços.
   
   Existem três níveis distintos de zoom que seu painel deve suportar. O nível totalmente ampliado ajuda você a avaliar o impacto do seu programa. O nível totalmente ampliado ajuda uma equipe individual a entender o trabalho restante. Um terceiro nível entre os dois ajuda os líderes organizacionais a responsabilizarem suas equipes (e apoia seu patrocinador de programa na formulação de pedidos concretos para responsabilizar esses líderes).

6. **Envie estímulos programáticos para as equipes atrasadas em seus objetivos.** As pessoas estão ocupadas. Nem sempre darão prioridade aos objetivos do seu programa. Alternativamente, eles podem fazer um trabalho incrível para fazer as melhorias solicitadas, mas retroceder mais tarde com práticas obsoletas. Use estímulos para direcionar a atenção das equipes para o próximo trabalho que elas devem realizar em direção aos objetivos do seu programa. Lembre-se, a atenção é um recurso escasso! Se você desperdiçar o tempo das pessoas com um e-mail ou ping de estímulo, elas não prestarão atenção ao próximo.

7. **Revise periodicamente o status do programa com seu patrocinador.** Os programas estão tentando progredir em uma prioridade organizacional que não se alinha naturalmente com os objetivos das equipes. Muitas equipes lutam para sair de sua priorização local para realizar prioridades globais. É aqui que é essencial revisar o progresso geral com seu patrocinador e apontá-los para as equipes que priorizam o trabalho do programa. Aproveitar eficazmente seu patrocinador para alinhar priorizações divergentes será essencial para seu sucesso.

Em muitos aspectos, um programa é apenas uma migração interminável, e <a href="http://lethain.com/migrations/">as técnicas que se aplicam às migrações funcionam também para programas</a>.

Se você acertar todos esses passos, estará executando um programa realmente ótimo. Isso pode parecer muito trabalho, e realmente é: muitos programas dão errado. As três principais causas de programas fracassados são:

1. administrá-lo puramente do ponto de vista de processo e se desconectar da realidade do que você está tentando realizar,
2. administrá-lo puramente do ponto de vista técnico e pensar que você pode pular as etapas essenciais de defender seu objetivo e ouvir as pessoas que você está tentando motivar,
3. tentar cobrir ambos os pontos de vista como uma única pessoa - não faça isso!

Um programa ruim é muito parecido com uma organização sem fins lucrativos ineficaz: o objetivo está correto, mas poucos fundos alcançam o objetivo pretendido. Não importa como você decide medir a qualidade técnica, a coisa mais importante a lembrar sempre ao executar seu programa de qualidade é que o programa não é o objetivo. O objetivo é criar qualidade técnica. Os programas organizacionais são massivos e constroem tanto impulso que a inércia os impulsiona para frente muito tempo depois de terem parado de funcionar. Mantenha seu programa enxuto o suficiente para cancelar e continue sendo autocrítico o suficiente para cancelá-lo se ele deixar de impulsionar a criação de qualidade.

## Comece pequeno e adicione lentamente

Quando você percebe que sua qualidade técnica real está consideravelmente atrás de sua qualidade técnica desejada, a reação natural é entrar em pânico e começar a implementar uma ampla variedade de técnicas e soluções. Despejar todos os ingredientes na panela, inevitavelmente, não funciona bem, e pior, você nem sabe quais partes manter.

Se você estiver lutando com a qualidade técnica - e todos nós estamos, com frequência - comece com algo pequeno e itere até que funcione. Em seguida, adicione outra técnica e itere também sobre ela. Construa lentamente em direção a algo que realmente funcione, mesmo que isso signifique enfrentar acusações de não estar se movendo rápido o suficiente. Quando se trata de sistemas complexos e interdependências, mover-se rapidamente é apenas uma questão de aparência. É o movimento metódico que faz o trabalho.

