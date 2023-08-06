# Visão Estratégica

A ideia é ter uma visão geral de como os contextos do domínio se encaixam, compreendendo suas interações e comunicações. Os contextos delimitados conversam entre si e podem se complementar durante o processo de desenvolvimento de software.

Para criar uma modelagem mais estratégica e ter uma visão ampla dos relacionamentos e funcionamento dos contextos, o "context mapping" é uma ferramenta útil. Esse mapeamento dos contextos ajuda a entender como organizar os times durante o desenvolvimento e início do projeto de software. Nesta etapa, ter uma visão mais elevada e estratégica é essencial para o sucesso do projeto.

## Context Mapping

A visão estratégica é fundamental para entender como os contextos se encaixam e se relacionam. O "context mapping" é uma ferramenta útil para mapear e compreender essas relações entre os contextos do domínio.

Ao realizar o "context mapping", é importante considerar diferentes tipos de relações entre os contextos, como:

- Parceria: Contextos que trabalham juntos, fornecendo e consumindo serviços um do outro.

- Shared Kernel (Núcleo Compartilhado): Contextos que compartilham um núcleo de sistema ou módulo.

- Cliente e Fornecedor: Um contexto fornece serviços para outro contexto.

- Upstream e Downstream: Contextos que têm uma relação de fornecedor e cliente, com o upstream ditando as regras e o downstream se adaptando.

- Conformista: Relação em que um contexto precisa se conformar com a forma como o outro contexto trabalha, geralmente em serviços de terceiros ou fornecedores externos. Para minimizar problemas de conformismo, pode-se utilizar a camada anticorrupção (ACL), que age como um adaptador entre contextos, facilitando futuras trocas de fornecedores.

O "context mapping" proporciona uma visão mais clara e estratégica da organização dos times, relacionamentos e interações entre os contextos, o que é especialmente relevante em sistemas maiores e complexos. Existem diversos padrões de "context mapping" que podem ser úteis para organizar e projetar os contextos de forma eficiente. 

## Padrões e Starter Kit

Os principais padrões de relações entre contextos apresentados são:

- **Partnership**: Relação de parceria, em que contextos trabalham juntos, fornecendo e consumindo serviços um do outro.

- **Shared Kernel**: Contextos que compartilham um núcleo ou módulo entre times.

- **Customer Supplier Development**: Relação de cliente e fornecedor, em que um contexto fornece um serviço que o outro consome, podendo ser upstream ou downstream.

- **Conformity**: Relação conformista, em que um contexto precisa se adaptar e conformar-se ao serviço do outro, sem poder alterá-lo.

- **ACL (Anti Corruption Layer)**: Camada anticorrupção que atua como um adaptador entre contextos, minimizando problemas de conformismo.

Além disso, existem outros padrões, como **Open Host Service** (um contexto que expõe serviços para outros sistemas) e **Published Language** (contextos que têm uma linguagem específica para a comunicação). Também o conceito de **Separated Ways**, quando contextos não se comunicam diretamente e têm suas próprias regras.

Cheatsheet de Context Mapping: https://github.com/ddd-crew/context-mapping/blob/master/README.md