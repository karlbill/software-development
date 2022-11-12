# Software Development
Resumo do livro Software Development, Design and Coding, de John F. Dooley.

## Fundamentos do Gerenciamento de Projeto
Tarefas envolvidas:
1. Planejamento
2. Estimativa e definição do cronograma
3. Gerenciamento de recursos
4. Supervisão
5. Revisão do projeto e apresentação
6. Retrospectiva

Gerente de projeto (tradicional): responsável pelo escopo, custo, estimativa, cronograma, qualidade, pessoal, comunicação, risco etc.
Projeto ágil: toda a equipe é responsável pelo gerenciamento do projeto.
> Obs: se houver um gerente de projeto, ele garantirá acesso aos recursos necessários, à aderência aos valores e princípios ágeis, facilitará a comunicação e blindará a equipe de interferências externas. Ele não gerenciará o dia-a-dia das operações da equipe. Apenas garantirá que não haja atraso nas decisões-soluções do gerenciamento.

### Planejamento do projeto
O planejamento é eterno porque o desenvolvimento está sempre em fluxo constante. 
> Um planejamento de projeto (plan-driven model) é um documento, escrito pelo gerente de projeto, aprovado e assinado pela equipe de desenvolvimento e o gerente superior. É um contrato sobre o que a equipe vai fazer e como vai fazer. Como o projeto será gerenciado. Consiste nas seguintes etapas:
1. Introdução e explicação do projeto
2. Organização da equipe
3. Análise de Risco
4. Requisitos de hardware, software e recursos humanos
5. Lista de tarefas, tamanho e esforços estimados
6. Cronograma de projeto
7. Monitoramento do projeto e mecanismos de relatório, conhecidos coletivamente como Supervisão de projeto

Obs: projetos baseados em planejamento farão uso de todas as etapas, enquanto projetos ágeis usarão apenas algumas.
Um planejamento de projeto é muito útil para detalhar como você fará as coisas mas... é estático. Seu gerente superior pensará que o projeto será executado exatamente como definido no planejamento.

Um planejamento de projeto ágil:
1. É baseado em features (construído em torno da ideia de colocar código rodando em produção rapidamente)
2. É organizado em iterações
3. É multi-camada (sabe-se que as coisas não estão definidas completamente desde o início)
4. É propriedade da equipe, não do gerente de projeto

### Organização do projeto:
Contém três elementos principais:
1. Como você vai organizar a equipe
2. Qual modelo o projeto irá usar
3. Como o projeto vai ser executado no dia-a-dia

A metodologia ágil simplifica esses três elementos porque as equipes ágeis são auto-organizadas, elas são pequenas e uma de suas principais ideias é o compartilhamento de responsabilidades. Os desenvolvedores ágeis não se segregam a partir das partes de código em que estão trabalhando ou baseado em suas habilidades. Eles compartilham o código, o teste e a expertise. Estão constantemente aprendendo e melhorando suas habilidades. 
> Não importa qual metodologia (XP, Scrum, Crystal, feature-driven etc), os projetos ágeis são iterativos, com ciclos de desenvolvimento curtos e produzem códigos funcionais ao final de cada ciclo. A maioria trabalhará com reuniões diárias, pelo menos integrações diárias e algum tipo de compartilhamento de programação, como pair programming. Os desenvolvedores passam a maior parte do tempo escrevendo e rodando testes unitários.

### Análise de Risco
O que pode dar errado? Qual é a pior coisa que pode acontecer? O que será feito se tal coisa acontecer?
Variáveis a observar:
  - Deslize no cronograma: há reuniões diárias em projetos ágeis, o que pode evitar que esse tipo de atraso ocorra, visto que pode ser notado imediatamente e as ações devidas serem imediatamente tomadas.
  - Taxa excessiva de defeitos: de um ponto de vista ágil, o melhor a se fazer é parar, olhar em volta e encontrar a causa raíz dos defeitos antes de adicionar novas funcionalidades. 
  - Má compreensão dos requisitos: clientes vivem no mundo do domínio da aplicação, enquanto os desenvolvedores entendem como o produto irá funcionar de um ponto de vista técnico. Para evitar desentendimento, os clientes devem estar o mais próximo possível da equipe de desenvolvimento.
  - Mistura de requisitos: em processo ágil, a equipe de desenvolvimento mantém o controle da lista de prioridades (Product Backlog no Scrum) e apenas ajusta essa lista após a Sprint (Scrum) ou após uma iteração (XP).
  - Sobrecarga: dê trabalho interessante aos desenvolvedores; um ambiente prazeroso; controle sobre seus cronogramas. A melhor maneira de mitigar a sobrecarga é espalhar o conhecimento do projeto entre todos os membros da equipe. Princípios como Responsabilidade de código compartilhada e técnicas como Pair Programming funcionam nesse sentido.
  
Sugestão de leitura: Peopleware, de Tom DeMarco.

> Uma vez que você tenha listado os riscos do projeto, você precisa endereçá-los e pensar sobre duas coisas: como evitá-los e como mitigá-los.
Evitar: defina um cronograma flexível, faça revisões de código, congele requisitos cedo, entregue com frequência, faça pair programming etc.
Mitigar (o que fazer se o pior cenário acontecer): remova as features da entrega, pare o trabalho de novas features e faça uma caçada ao bug, negocie novas features para entregas futuras e por aí vai.

### Requisitos de recursos
Quantas pessoas serão necessárias? Quantos computadores? Quais softwares serão usados no desenvolvimento? Todo mundo está treinado? 
> Você precisará de um sistema de gerenciamento de configuração e uma máquina isolada, não importa que tipo de modelo você está usando.
>
> Questões sobre tamanho da equipe, data de início e fases do projeto podem ser respondidas após as estimativas de esforços e cronograma.

### Estimativas de tarefas
O clássico problema do ovo e da galinha: você não pode fazer uma estimativa até ter uma decomposto detalhadamente as features ou histórias de usuários em tarefas. Faça do design sua primeira prioridade uma vez que você tenha alguma ideia dos requisitos. 
> Se você escolher uma lista pequena de requisitos de alta prioridade e então projetar uma solução para esse conjunto de features, então você pode fazer uma estimativa de esforço dessa iteração. Você precisa quebrar a feature em tarefas implementáveis antes que possa fazer uma estimativa de esforço.

Você tem que partir seu trabalho em tarefas que não sejam maiores do que uma semana para serem concluídas. 
> Nunca faça estimativas em qualquer unidade alé de pessoa-horas. Você será tentado a trabalhar comm pequenos incrementos de horas e você quebrará suas tarefas maiores em menores, a ponto de saber realmente como resolvê-la. O tamanho sempre deve vir primeiro. Tamanho pode se referir a muitas coisas: módulos funcionais, números de classes, de métodos, de objetos, ou **linhas de código não comentadas (KLOC)**.

Técnicas para estimativa de esforço: COCOMO II, Function Point Analysis e Delphi method.
> Mantra da estimativa: tamanho em primeiro lugar, depois estimativa de custo e esforço, só então o cronograma.

Explicação para o método Delphi (rápido e relativamente eficiente): 
1. reúna os três mais experientes desenvolvedores e dê a eles as tarefas detalhadas. 
2. Peça a eles para te dar 3 números para cada tarefas: a menor, a maior e a quantidade normal de tempo que a tarefa deveria consumir, todas em pessoa-horas.
3. Reúna os dados e faça a média (da melhor estimativa pelos melhores desenvolvedores). Utilize essa média como a estimativa de esforço oficial e comece a definir o cronograma.
> Gerentes nunca devem fazer as estimativas de desenvolvimento, mesmo se tiver sido desenvolvedor no passado (a menos que esteja profundamente envolvido no processo de desenvolvimento).

Pelas minhas experiências, a estimativa de esforço realizadas com toda a equipe, através de técnicas como Poker plan não são muito úteis. Em geral, os desenvolvedores menos experientes acabam seguindo os mais experientes, à medida que algumas tasks são estimadas e começa-se a se ter uma noção dos valores que cada desenvolvedor costuma escolher. Sempre fui muito crítico em relação ao Poker Plan, pela falta de personalidade das pessoas envolvidas no processo mas não conhecia uma estratégia melhor. Acredito que a resposta para minha crítica seja o método Delphi.

### Cronograma de Projeto
Uma vez tendo as estimativas de tempo para as tarefas da primeira iteração e tendo uma estimativa de recursos/pessoas necessárias, você pode criar o Cronograma. Muitas coisas precisam ser levadas em consideração:
  - Verifique com os desenvolvedores as dependências entre as tarefas: algumas tarefas não podem ser iniciadas sem que outras sejam concluídas.
  - Descubra qual é o seu ciclo de trabalho: realisticamente, de cada oito horas diárias, de duas a quatro horas são consumidas com outras coisas, então seu ciclo de trabalho pode ser reduzido a 50%. Pode variar baseado na cultura da empresa.
  - Leve em consideração os fins de semana, férias, falta por doença, treinamento
  - Você não pode enquadrar um desenvolvedor para trabalhar em duas tarefas ao mesmo tempo. 
> Utilize um software de definição do cronograma. Para projetos pequenos, uma simples técnica de planilha pode ser o bastante (técnica de Joel Spolsky). </br>
> Softwares para plan-driven projects: MS Project, Fast Track Scheduling, Basecamp, Merlin </br>
> Softwares para projetos ágeis: Jira, Pivotal Tracker, Trello </br>
> Em projetos ágeis, como Scrum, em que se utiliza tempos curtos para Sprints e você precisa conhecer as prioridades de cada História do Usuário no Backlog do Produto, e como elas se relacionam umas com as outras, e como você deve ter uma boa estimativa de quanto tempo cada tareffa levará, e você precisa rastrear o progresso do número de tarefas no Backlog da Sprint diariamente - ter um software que rastreie as dependências pode ser o diferencial entre cumprir a Sprint ou não.

Exemplo de uma planilha de cronograma:

![image](https://user-images.githubusercontent.com/39681960/201451948-22cfab3c-2898-4339-8571-d3192f1ebd93.png)

Essa é uma estratégia útil para projetos menores com uma quantidade bem limitada de tarefas. Para que essa planilha funcione, as tarefas precisam ser granulares e pequenas em termos de esforço. Cada desenvolvedor deve ter uma planilha separada ou ser adicionada uma coluna com o nome do desenvolvedor, como na imagem acima. 
> A coluna 9 da planilha é uma medida de Velocidade (termo da metodologia XP), definida como uma estimativa de esforço de uma tarefa, dividida pelo esforço atual (Estimativa original / Tempo real gasto). Se velocidade > 1, a estimativa foi superestimada; se abaixo, foi subestimada. Idealmente, deve ser igual a 1. </br>
> Algumas ferramentas de gerenciamento de projeto permitem utilizar uma variável *magnitude*: dar uma pontuação para cada tarefa. O motivo para isso é dar uma ideia da precisão das estimativas realizadas e ser uma medida auxiliar para as próximas estimativas.







## Referência bibliográfica:
DOOLEY, John F., Software Development, Design and Coding, Apress, 2017, 2nd Edition.
