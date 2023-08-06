# Dominios Subdominios e Contexto

## Dominios vs Subdominios

O Domain Driven Design (DDD) nos leva a pensar inicialmente no domínio, o coração da aplicação. Porém, ao entender melhor o negócio, podemos dividir o domínio em subdomínios menores. O Core Domain é o mais importante, o diferencial competitivo da empresa. Há também os subdomínios de suporte, que apoiam o Core Domain, e os subdomínios genéricos, que auxiliam no dia a dia, mas não possuem diferencial competitivo significativo. O DDD é mais do que padrões de projeto; é a exploração e encaixe desses domínios e subdomínios durante o desenvolvimento.

## Espaço do problema vs Espaço da solução

No Domain Driven Design (DDD), existe a distinção entre o Espaço do Problema e o Espaço da Solução. O Espaço do Problema é a visão geral do domínio e suas complexidades, enquanto o Espaço da Solução é a modelagem desse domínio para a resolução dos problemas. O DDD destaca a importância de focar na modelagem do domínio para delimitar subdomínios e transformá-los em contextos delimitados, que se tornam os pontos de trabalho na solução do software. A exploração do domínio leva à modelagem e à definição dos contextos, permitindo atacar os problemas de forma mais estruturada.

## O que é um Contexto Delimitado (Bounded Context)?

Um contexto delimitado é uma divisão explícita dentro do modelo de domínio em DDD. É como se fosse uma fronteira que define uma parte específica do domínio que está sendo modelada. Essa delimitação é estabelecida por meio de uma linguagem de comunicação específica utilizada dentro desse contexto, chamada de linguagem ubíqua ou linguagem universal. A linguagem ubíqua é um dos principais indicadores para determinar em qual contexto delimitado se está. Contextos delimitados são fundamentais para a modelagem de domínio e têm importância em cenários complexos, onde diferentes áreas trabalham em conjunto e possuem terminologias específicas. O entendimento e identificação desses contextos são cruciais para o sucesso do DDD.

### Contextos

O contexto é rei em DDD, pois determina a área da empresa em que estamos trabalhando e o tipo de problema que estamos resolvendo. Cada contexto delimitado possui uma linguagem específica, onde palavras podem ter significados diferentes em contextos diferentes. A identificação dos contextos é crucial para a modelagem adequada do domínio. Quando palavras iguais têm significados diferentes, provavelmente estão em contextos distintos. Da mesma forma, quando palavras diferentes representam a mesma coisa, provavelmente estão em contextos diferentes. A compreensão dos contextos é essencial para evitar ambiguidades e garantir a correta modularização do sistema. Em um sistema monolítico, diferentes contextos exigem a criação de entidades e áreas distintas para evitar conflitos de significado.

## Elementos transversais

Em DDD, mesmo em contextos delimitados diferentes, pode haver elementos transversais, como a mesma entidade (por exemplo, "cliente") sendo usada em diferentes contextos com perspectivas distintas. Esses elementos têm o mesmo nome, mas representam coisas diferentes. É fundamental entender que cada contexto deve ser modelado de acordo com suas próprias perspectivas e informações relevantes.

Ao desenvolver um sistema monolítico, é importante criar entidades específicas para cada contexto, evitando a criação de uma única entidade gigante que tenta atender todos os contextos em que o elemento está presente. A falta de delimitação de contextos pode levar a sistemas complexos e difíceis de manter.

A perspectiva diferente em cada contexto faz toda a diferença na hora do desenvolvimento do sistema. Ao mapear essas perspectivas e organizar as ideias de forma clara, é possível evitar confusões e manter a aplicação organizada.