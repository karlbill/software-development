# Software Development
Resumo do livro Software Development, Design and Coding, de John F. Dooley.

## Princípios de Design
Dividiremos os problemas de software em duas camadas distintas:
  - Problemas maldosos (camada superior): surgem de domínios fora da ciência da computação e tendem a ser problemas em aberto, não bem-definidos. Requerem muito trabalho.
  > Não é compreendido até a criação de uma solução </br>
  > Não há uma regra que diga que a solução final foi encontrada: não é um problema de certo ou errado mas, sim, melhor ou pior. </br>
  > É essencialmente inusitado e único </br>
  > Toda solução é uma operação de um único tiro </br>
  
Obs: Processamento de palavras é o problema maldoso mais óbvio que existe: você pode pensar que um processador de palavras precisa apenas inserir, cortar e colar texto, manipular parágrafos e imprimir o texto. Assim que você termina seu processador e libera a versão, você é inundado com novas requisições de features como checagem de caracteres, notas de rodapé, múltiplas colunas, suporte para diferentes fontes, cores e estilos etc. Isso nunca tem fim.
  
A maioria das pessoas irá seguir uma solução linear para resolver esse tipo de problema, trabalhando de maneira Top-Down do problema à solução.
![image](https://user-images.githubusercontent.com/39681960/201549579-6c8162ba-5ad9-44ba-993d-7734906e7cee.png)

Verdadeiros solucionadores de problemas dessa natureza tendem a usar uma abordagem que varia da análise de requisitos ao modelo de solução, iterando entre estes até obter uma solução boa o suficiente.
![image](https://user-images.githubusercontent.com/39681960/201549665-6efe4b9c-0d1e-4306-8003-51dfd727d832.png)

Outro problema maldoso é o de desenvolvimento de uma aplicação web: o cliente não tem ideia de como gostaria que a página web fosse. Desse modo, qualquer que seja sua primeira apresentação, não será precisamente o que ele quer. O problema não estará completamente compreendido até que você o tenha concluído. À medida que seus protótipos são construídos, mais features serão solicitadas - então, o problema não tem regra de parada, não há resposta certa. Há apenas a resposta "boa o suficiente". 

  - Problemas domesticados (camada inferior): claramente definidos. Problemas que dão a sustentação em termos de Estrutura de Dados e Algoritmos para os problemas maldosos de outros domínios.
    - Características:
    1. Formulação bem-definida e estável
    2. Um ponto de parada definido
    3. A solução pode ser objetivamente avaliada como certo ou errado
    4. pertence a uma classe de problemas similares
    5. As soluções podem ser facilmente testadas e abandonadas
    6. Acompanhado de um conjunto limitado de alternativas de soluções.
    
  > Exemplo: ordenação de valores em uma lista
    - Claro e facilmente estabelecido: ordenação crescente ou decrescente
    - Um ponto de parada definido: quando a lista estiver ordenada
    - Objetivamente avaliado: a lista está ordenada ou não
    - Pertence a uma classe de problemas similares: ordenação de Strings, de Inteiros etc
    - Possui soluções que podem ser facilmente testadas e abandonadas
    - Tem uma lista limitada de alternativas de solução: algoritmos de ordenação conhecidos.
    
### O processo de Design
Pode parecer uma bagunça, visto que é dinâmico e mudará à medida que for evoluindo e seu conhecimento sobre o projeto for aumentando.
Projetos são limitados por tempo, então você deve saber quais requisitos priorizar e ter a habilidade de negociar com o cliente (trade-off).
Projeto é heurística. Essas heurísticas e padrões dão ao bom designer maior rapidez em atingir o coração de um Wicked problem.
Design evolui: para qualquer tipo de problema, os requisitos irão mudar com o passar do tempo. A sacada é criar uma arquitetura de software que comporte as mudanças vindouras.
    
Características desejáveis de Desing:
  - Fortemente ligada ao propósito: seu projeto deve funcionar, ou seja, satisfazer os requisitos. Não adicione requisitos você mesmo - o cliente fará isso por você.
  - Separação de conceitos: relacionado à Modularidade (separação do projeto em partes funcionais) para facilitar a manutenção.
  - Simplicidade: mantenha seu projeto e código tão simples quanto possível, o tempo todo (Refatoração).
  - Facilidade de manutenção: erros acontecem ao longog de todo o processo de desenvolvimento (requisitos, análise, código e teste).
  - Baixo acoplamento: separação do projeto em Módulos (ou em Classes, na Orientação a Objetos). Módulos fortemente acoplados compartilham dados e procedures. Isso aumenta a carga de trabalho e propicia maior quantidade de erros ao Módulo. O Baixo Acomplamento, por outro lado, faz com que os módulos se conectem via Interfaces, escondendo os detalhes de implementação. Dessa forma, as mudanças ficam isoladas ao módulo correspondente e os erros dificilmente são propagados entre eles.
  - Alta coesão: é o grau de que cada módulo está auto-contido em relação tanto aos dados que armazena quanto às operações que realiza sobre os dados. Os dados de que uma classe precisa são definidos dentro da própria classe, assim como suas operações.
  - Extensibilidade: ramificação da Simplicidade e Baixo Acoplamento. Está relacionado à facilidade de adição de novas features ao projeto.
  - Portabilidade: capacidade que seu projeto tem de rodar em ambientes diversos.
  
### Heurísticas de Design













## Referência bibliográfica:
DOOLEY, John F., Software Development, Design and Coding, Apress, 2017, 2nd Edition.
