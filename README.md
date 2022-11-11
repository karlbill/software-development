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







## Referência bibliográfica:
DOOLEY, John F., Software Development, Design and Coding, Apress, 2017, 2nd Edition.
