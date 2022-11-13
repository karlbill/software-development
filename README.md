# Software Development
Resumo do livro Software Development, Design and Coding, de John F. Dooley.

## Arquitetura de Software
"Noção dos elementos principais de um sistema, as peças que são difíceis de mudar. A fundação sobre a qual todo o resto deve ser construído." (Martin Fawler)

Uma vez que se tenha definido o que se quer construir, agora passamos a pensar em COMO isso será construído. Existem dois níveis de Software Design:
1. Detailed Design:
  - Quais operações são necessárias? Quais Estruturas de Dados? Quais algoritmos? Como o banco de dados será organizado? Como a Interface com o usuário deve ser? Quais são as sequências de chamada?
2. Style Design:
  - Essa ênfase no estilo é sobre o que a Arquitetura de Software trata. Arquitetura de Software é um conjunto de ideias que te dizem qual fundação é a certa para seu programa. 
> "Quando o tamanho e a complexidade do sistema cresce, o problema de design vai além de algoritmos e estruturas de dados: projetar e especificar a estrutura de todo o sistema surge como um novo tipo de problema...isso é o nível de design da Arquitetura de Software." (Garlan & Shaw)

Diferentes tipos de programas, de diferentes domínios, nos levarão a diferentes estilos de arquitetura (Padrões Arquiteturais, com muitas características de Padrões de Projeto).

A Arquitetura de Software é representada geralmente como grafos de caixa preta, onde os nós são Estruturas Computacionais e as ramos são os condutores de comunicação (fluxo de dados, objeto passado como mensagem, chamadas de procedures) entre as estruturas.
> Notação mais comum: UML

### O programa principal - Padrão da Subrotina Arquitetural

![image](https://user-images.githubusercontent.com/39681960/201500587-14ecd8fc-3efb-45a6-a56b-64545a693240.png)

É o padrão arquitetural mais velho e tradicional, formalizado por Niklaus Wirth em 1971, no artigo "Program Development by Stepwise Refinement", definindo a metodologia de divisão de um problema de maneira top-down.
1. Você começa com um grande problema e então o divide em várias partes menores, semi-independentes pedaços do problema original. </br>
2. Uma vez dividido em várias partes, olhe para cada parte separadamente e continue dividindo até chegar em um problema tão pequeno que a solução seja óbvia. Nesse momento, você começa a programar. </br>
3. Você quebra o problema de cima pra baixo e começa a programar de baixo para cima.

### Arquitetura Pipe-and-Filter

![image](https://user-images.githubusercontent.com/39681960/201500687-14389baa-28de-4f3c-ad3a-68a60cdb325f.png)

Os componentes computacionais são chamados Filtros (como transdutores que recebem uma entrada, transformam a entrada de acordo com um ou mais algoritmos e geram uma saída para os condutores). As entradas e saídas são chamadas Pipes. Os Filtros devem ser componentes independentes.
> Você pode unir os filtros em configurações diversas para produzir diferentes resultados. 
1. Exemplo clássico: shell Unix -> grande número de pequenos programas que executam uma única função e podem ser linkados usando o mecanismo de pipe do Unix. </br>
2. Programming Pearls (Jon Bentley's book): dado um dicionário de palavras em inglês, encontre todos os anagramas em um dicionário. Isto é, encontre todas as palavras que sejam permutações de outras palavras.
  - Todos os anagramas têm o mesmo número de letras. Se você ordenar cada String, todas as palavras que sejam anagramas terão a mesma ordenação. Então, basta manter uma forma de rastreamento de cada palavra antes da ordenação para retornar uma saída com essas palavras originais.
  - Como essa solução se relaciona com a arquitetura Pipe-and-filter? Solução em Unix:
  ![image](https://user-images.githubusercontent.com/39681960/201501449-071fa69e-d8ce-49ab-bbd6-37a38614e566.png)
    - Todas as características do padrão estão nesse exemplo: componentes computacionais independentes  que realizam uma transformação nos dados de entrada e se comunicam transmitindo os dados transformados em sua saída para a entrada do próximo componente.
    










## Referência bibliográfica:
DOOLEY, John F., Software Development, Design and Coding, Apress, 2017, 2nd Edition.
