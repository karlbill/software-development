# Software Development
Resumo do livro Software Development, Design and Coding, de John F. Dooley.

## Software Process Models
Não importa se grande ou pequeno, quantas pessoas trabalham no projeto, todos os programas passam pelas mesmas etapas:
1. Concepção
2. Levantamento de Requisitos / Exploração / Modelagem
3. Projeto
4. Codificação e debug
5. Teste
6. Entrega
7. Manutenção / Evolução do Software
8. Aposentadoria

Todo processo de desenvolvimento é uma variação de um dos dois tipos fundamentais (2 classes de modelos de gerenciamento de projeto): 
* Fazer o ciclo completo (pelo menos de 2 a 7) antes de iniciar uma nova versão do produto. (Tradicional plan-driven model)
* Fazer um ciclo parcial (geralmente de 3 a 5) e iterar por essas etapas várias vezes antes de prosseguir com a entrega. (modelo ágil)

1. Modelo orientado a planejamento: 
  - Estrito no sentido de etapas do processo
  - Fases mais claramente definidas
  - mais requisitos para cumprir em uma etapa
  - mais documentação em cada etapa
  - tende a funcionar melhor em contratos longos para novos softwares com entregas bem-definidas
  
2. Modelo ágil:
  - Inerentemente incremental: a ideia é de que entregas frequentes produzem um sistema mais robusto do que aqueles maiores e menos frequentes.
  - Tende a ter menos documentação
  - Código é o que se produz, então os esforços do desenvolvedor devem focar nisso.
  
Todo projeto deve escolher o que melhor funcione para sua aplicação, baseado em: 
  - domínio da aplicação
  - tamanho do projeto
  - experiência da equipe 
  - tempo de vida do projeto
  
4 fatores (variáveis) que todo projeto de desenvolvimento de software tem em comum:
  * Custo: o mais restritivo --> tamanho da equipe, tipos de ferramentas disponíveis;
  * Tempo: cronograma de entrega --> em geral, imposto a você;
  * Qualidade: número e gravidade de defeitos que você está lidando para entregar o software --> sacrificar a qualidade reduzindo o cronograma de entrega gerará mais tempo para corrigir as novas entregas e afetará sua credibilidade bastante;
  * Features (escopo): a variável mais importante do ponto de vista do cliente. A variável sobre a qual você como desenvolvedor tem maior controle.
  
### Um modelo que não é um modelo: Programar e Corrigir (Code and Fix Model)
Nesse modelo não há requisitos formais, nenhuma documentação exigida, nenhuma garantia de qualidade, nenhum teste formal. Gasta-se o mínimo de tempo no entendimento do problema e então se começa a programar:
1. Compile seu código e veja se funciona.
2. Se não, corrija o primeiro problema que encontrar e tente novamente.
3. Continue esse ciclo de compilar - rodar - corrigir até o programa fazer o que você quer, sem erros fatais e então o entregue.

Essa é uma forma horrível de fazer protótipos rápidos e sujos. É útil para validar decisões de arquitetura e para mostrar uma versão rápida de um projeto de UI (prova de conceito). Para qualquer outro tipo de sistema, é um modelo muito perigoso de se trabalhar.

### Modelo Waterfall
O primeiro e mais tradicional modelo orientado a planejamento. Contém todas as fases do ciclo de vida padrão. Funciona muito bem com análise e levantamento de requisitos, projeto arquitetural, detalhes de projeto, codificação, debug, teste e integração de sistemas, entrega e manutenção. Requer uma documentação detalhada em cada etapa. Encerra cada fase do processo.

![image](https://user-images.githubusercontent.com/39681960/201400082-fee5b11d-98d6-42b7-8211-dd0fc770a1c9.png)

2 problemas fundamentais com o modelo Waterfall: 
  - geralmente você precisa terminar a fase N para iniciar a fase N + 1: você precisa destrinchar todos os requisitos antes de iniciar o projeto arquitetural, por exemplo.
  - fundamentalmente baseado em uma mentalidade de linha de montagem: não há como voltar e retrabalhar seu projeto se você encontrar um problema durante a implementação.

Obs: na teoria é um modelo muito bom. Ele isola as diferentes fases do ciclo de vida e te força a pensar sobre tudo o que é necessário saber antes de seguir em frente. Boa estratégia para projetos longos e para equipes inexperientes inseridas em um projeto bem definido.

### Modelos Iterativos
O mais tradicional: Prototipação Evolutiva --> prioriza os requisitos recebidos, produzindo sucessivas versões de ricas features do produto. Cada versão é refinada a partir do feedback do cliente e dos testes de integração do sistema. Muito usado em ambientes dinâmicos ou com requisitos ambíguos, com baixo entendimento do domínio da aplicação. Evoluiu para o moderno processo de desenvolvimento ágil.

![image](https://user-images.githubusercontent.com/39681960/201403753-c9124936-d5c8-4a49-a1c1-54d4bacf97d6.png)

Nesse modelo se reconhece a dificuldade de se obter todos os requisitos de um projeto desde o começo, que são levantados juntamente com o feedback feito pelos clientes a partir das features iniciais entregues. Provê visibilidade de progresso tanto para o cliente quanto para o gerente de projeto, facilitando a priorização de requisitos ao munir os usuários finais e clientes.

Pontos negativo: 
  - pode ser conduzido a cronogramas irreais, superfaturamento e superestimar as expectativas de progresso. 
  - o projeto envolve trabalho extra uma vez que os requisitos mudem e há a possibilidade de um mal projeto, que geraria muito retrabalho e uma corrente de descumprimento de cronograma e crescente dificuldade de corrigir os bugs pós-entrega.
  
Obs: Funciona bem para equipes pequenas e muito experientes, que estejam entrosadas.
  
### Risco
É o problema mais básico e pode se manifestar de diversas maneiras: deslize no cronograma, cancelamento do projeto, aumento na taxa de defeitos, má compreensão dos problemas de negócio e esgotamento da equipe. 
A metodologia ágil busca minimizar os riscos controlando as quatro variáveis do desenvolvimento de software, dando maior controle aos desenvolvedores sobre essas variáveis mas, especialmente, sobre o controle do escopo do projeto. 

### Metodologia Ágil



## Referência bibliográfica:
DOOLEY, John F., Software Development, Design and Coding, Apress, 2017, 2nd Edition.







