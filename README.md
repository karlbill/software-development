# Software Development
Resumo do livro Software Development, Design and Coding, de John F. Dooley.

## Requisitos
"A função mais importante que um construtor de software executa para o cliente é a extração iterativa e refinamento dos requisitos do produto."
(Fred Brooks)

Antes de começar a programar, você precisa saber o que você vai construir. Requisitos são: uma lista de coisas que você tem que implementar de modo a criar seu maravilhoso programa. Se você quiser ser um desenvolvedor produtivo, cometer menos erros e criar um bom e limpo projeto, você precisa de requisitos. E quanto mais detalhados, melhor.

Requisitos funcionais: a lista de features que os usuários verão e estarão aptos a usar quando eles rodarem seu programa. Em um processo orientado a planejamento, a saída das atividades de identificação dos requisitos é uma Especificação Funcional do que o sistema de software deveria fazer. Em um processo ágil, a saída é um conjunto de Histórias do Usuário que definem o Backlog do Produto.

4 tipos de requisitos:
* Requisitos do usuário
* Requisitos de domínio
* Requisitos não-funcionais
* Não-requisitos

### Requisitos de Usuário
Geralmente expresso em linguagem natural que descreva qualquer elemento de interação no programa. Ex: descrição de layouts de tela, caixas de diálogo e menus.
> Expresse os requisitos de usuário como cenários e com uma descrição detalhada tela-a-tela. Utilize imagens o quanto quiser.

### Requisitos de Domínio
São impostos a você pelo domínio da aplicação. Geralmente são considerados "camada intermediária", porque são o coração de uma aplicação, abaixo da interface com o usuário e acima do Sistema Operacional, da rede ou do banco de dados. 
> Implementados como classes separadas e bibliotecas com suas próprias APIs.

### Requisitos não-funcionais
São limitações nos serviços e funções do programa e também expectativas sobre a performance. Podem não ser visíveis ao usuário mas tem efeito sobre a experiência desses usuários (UX). Ex: uso de memória, privilégios de acesso, requisitos de segurança, tempo de resposta etc.

### Não-requisitos
O que não será feito no projeto. Na fase de requisitos, o mais importante a ser feito é *gerenciar as expectativas*. Você precisa dizer aos stakeholders de um projeto o que o programa irá e o que ele não irá fazer.

## Levantamento de Requisitos em um projeto orientado a planejamento
A Especificação Funcional descreve o que o programa irá fazer, completamente do ponto de vista do usuário: especifica telas, menus, diálogos... </br>
Uma Especificação Técnica descreve detalhes da implementação interna do programa: estrutura de dados, algoritmos, modelos de dados, escolha de linguagens de programação etc.
> A metodologia ágil também escreve Especificação Funcional: Histórias de usuário que mostram o que o programa fará. Isso é especificação.

Obs: escreva o que o seu programa fará antes de começar a programar!

Requisitos funcionais devem ser escritos em linguagem natural (Hipótese da Relatividade Linguística de Sapir-Whorf): a linguagem não apenas determina o que você diz, ela determina o que você consegue dizer (e pensar). A linguagem que você utiliza determina que tipo de pensamento você é capaz de ter.

Recomendação de leitura: Notation as a tool of thought (Kenneth Iverson)

Elementos que uma especificação funcional deveria ter:
1. Overview
  - Resumo executivo: um ou dois parágrafos do que o programa deve fazer

2. Aviso
  - Seu aviso deve ser do tipo: "Essa especificação está tão completa quanto deveria para essa entrega. Se você acha que algo está errado ou faltado, envie um email para o autor e nós iremos considerá-lo para a próxima entrega."

3. Nome do autor
  - O responsável pela especificação funcional: nem um comitê, nem uma equipe, uma pessoa. Geralmente, o gerente de desenvolvimento ou de projeto. 
  - Gerentes de projeto precisam ter habilidades técnicas e ser muito bons em lidar com os stakeholders para obter o consenso acerca das especificações funcionais.

4. Cenários de uso
  - Escreva cenários como Histórias de Usuário
  - Na metodologia XP, os usuários são parte do projeto; no Scrum, não são parte do projeto mas são encorajados a estarem próximo do time.
  - UML possui os Use Cases para a construção de cenários
  - Utilize imagens: valem mais do que mil palavras

5. Assunto em aberto
  - Separe o que você ainda não sabe nessa seção: no futuro, irão para a seção de requisitos ou de não-requisitos
  - Ao final, essa seção deve estar vazia

6. Ideias de Projeto e de Novas Features
  - Tome nota das ideias que forem surgindo ao longo do projeto
  - Se você quiser que seus requisitos estejam em dia, você deve ter algo como um documento de Backlog: todos os requisitos que você vai considerar para a próxima entrega do produto

Obs: o único momento em que a especificação funcional está completa, é quando você libera a entrega. Não gaste tempo tentando extrair todos os requisitos de seu cliente. Defina um tempo limite e siga em frente.

### Levantamento de Requisitos em um projeto ágil
Em um modelo ágil, não há Especificação Funcional. Os requisitos mudarão, então a equipe deve abraçar a mudança. O cliente é parte da equipe, então a equipe pode ter um feedback imediato acerca das implementações das features. Isso gera maior confiança de que o conjunto de requisitos escolhidos é o conjunto certo.
> A ideia chave do levantamento de requisitos é a História do Usuário: uma descrição de alguma feature ou cenário que o cliente quer executar para realizar algum tipo de trabalho. </br>
> Modelo: "Como um <função>, eu quero fazer <ação>, então <razão/benefício>." </br>
> Com esse modelo, você tem o QUEM, ,O QUE e POR QUÊ do requisito.

Componentes de uma História de Usuário: 
1. Cartão: contém o texto da história. Pode ser escrito em um Post-it, um pedaço de papel etc. Não é muito detalhado.
2. Conversa: discussão sobre o que o dono do produto realmente quer com a história, estimativa de tamanho e de prioridade relativa.
3. Confirmação: critério de aceitação da história, geralmente escrito atrás do cartão. Terminará com Testes de Aceitação.

* INVEST (Acrônimo para as características de uma boa História de Usuário):
  - Independente: uma história de usuário não pode depender de outra história de usuário. (Ex: bolo multi-camadas)
  - Negociável: provê ao desenvolvedor um objetivo e permite que o proprietário e o desenvolvedor criem uma implementação funcional
  - Valorosa (para o cliente): se o time decide que a história deve ser dividida em duas ou mais, cada uma delas deve prover valor ao cliente.
  - Estimável: crítico para o proprietário do produto. Estimativa permite que o time foque no tamanho da história, é umam parte da Negociação na Conversa. Deve ser a primeira etapa ao se decompor uma História em Tarefas implementáveis.
  - Small (Pequena): deve ser implementada em uma única Sprint ou Iteração, idealmente com um esforço de 8 horas/pessoa ou menos. 
  - Testável: No modelo ágil, essa prática é implementada pelo TDD e Critério de Aceite (escrito pelo P.O.). Ao rodar os testes unitários criados pelos desenvolvedores e os testes confirmem que as tarefas estão corretas, então a História é marcada como Done.
> É também uma forma de testar os requisitos não funcionais como: performance, tempo de resposta, usabilidade etc.

### Product Backlog
A quantidade de histórias geradas pelo PO e acordadas com o time de desenvolvimento é adicionada a uma lista com o total de coisas a serem feitas para a criação do produto, chamada Backlog do produto.
Plan-driven: especificação funcional
Agile methodology: pilha de cartões (preliminarmente, definido pelo PO) -> cartões são adicionados, removidos e divididos em outros cartões, constantemente.
> É tarefa do PO decidir quando o produto está concluído e deve ser lançado.

### Tarefas SMART
Tarefas são o trabalho a ser feito de maneira a implementar as Histórias de Usuário. No Scrum, cada tarefa recebe uma pontuação baseada em seu grau de dificuldade. Ao final, a lista de tarefas é apresentada ao PO que aprova ou sugere mudança na prioridade de alguma história.
> Dividir as Histórias em Tarefas é responsabilidade da equipe de desenvolvimento, como parte do planejamento de uma Sprint ou Iteração.

Cada tarefa deve atingir um objetivo, caracterizado pelo acrônimo SMART:
1. Specific: Histórias de usuário podem ser gerais mas as tarefas associadas a ela devem ser específicas a ponto de serem implementadas, incluindo detalhes de Estruturas de Dados ou Interface com o usuário, por exemplo.
2. Mensurável: o time precisa saber quando todos os requisitos para as tarefas tiverem sido cumpridos. Quando? Pode ser definido de várias maneiras: "a feature funciona comoo listada na tarefa", "todos os testes unitários passaram", "os códigos foram revistos e integrados."
3. Alcançável: um desenvolvedor pode realizá-la no tempo de uma Sprint ou Iteração. 
> A ideia de Pair Programming se encaixa bem aqui.
4. Relevante: deve adicionar valor à Iteração para o cliente. 
> Se encaixa bem ao V do acrônimo INVEST.
5. Time-boxed: a tarefa, como estimada, pode ser finalizada dentro de uma Sprint ou Iteração.
> O número de pontos total assinado para as tarefas incluídas na Iteração é alcançável dentro da velocidade média da equipe.

### Sprint Backlog/ Iteraction Backlog
Quando as tarefas estiverem criadas e estimadas, elas serão adicionadas à Sprint Backlog ou Iteraction Backlog (XP). No Scrum, uma vez que a Sprint esteja definida, nenhuma tarefa pode ser adicionada, exceto pelos próprios desenvolvedores, durante a duração da Sprint. 
> Qualquer trabalho adicional deve ser colocada ao Product Backlog.
















## Referência bibliográfica:
DOOLEY, John F., Software Development, Design and Coding, Apress, 2017, 2nd Edition.
