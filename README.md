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




















