# Histórias de Usuário
As histórias de usuário especificam e descrevem ações na linguagem de negócio ou cotidiana, seja esta do usuário do sistema ou do usuário final. Também são utilizadas como base de escopos de projetos de software a partir das metodologias ágeis e de desenvolvimento de software. Resumidamente, as histórias de usuário são focadas no "quem", "o quê" e o "por quê" de um requisito, de forma simples e sem muitos detalhes para que a compreensão seja facilitada. Para facilitar ainda mais a compreensão, é certo criar uma história de usuário para cada tela do sistema.

### Exemplo:

"Sendo um **cliente**, quero **consultar** a lista de compras para **encontrar o eletrodoméstico** que reservei."

### Modelo de criação da História de Usuário:

**Sendo** *<persona>*
**Quero** *<funcionalidade>*
**Para** *<benefício>*

### Aplicando o "Quem", "O quê" e o "Por quê":

**Sendo** o atendente de uma biblioteca - *QUEM?*
**Quero** registrar a devolução de um livro no sistema - *O QUÊ?*
**Para** que o livro retorne a ficar disponível e volte a ser emprestado por outras pessoas - *POR QUÊ?*

## Metodologia INVEST

Para aprimorar a qualidade das histórias de usuário, usa-se a metodologia INVEST, que consiste em:

**Independente (Independent):** 
Histórias de usuário devem ser independentes umas das outras e completas nelas mesmas. Deve também ser desenvolvida, testada e até mesmo entregue de forma individual.

**Negociável (Negotiable):**
Como a história do usuário ainda é algo abstrato, é importante que a HU tenha um ponto de partida de escopo variável, ou seja, que possa ser negociável. Partindo dessa função, é possível discutir sobre a prioridade das funcionalidades dentro da HU.

**Valioso (Valuable):** 
A intenção da história de usuário é entregar um resultado concisa ao usuário e não apenas uma teoria para solucionar seu problema.

**Estimável (Estimable):** 
As histórias estimáveis devem ser sucintas e claras, com detalhes o suficiente e bem explicadas em nível técnico e de negócio. 

**Pequeno (Small):** 
É adequado que a história seja pequena, a fim de que seja concluída em apenas uma iteração. Para isso, também podem ser divididas em histórias menores.

**Testável (Testable):** 
A história deve sempre ser testada e evitar muitos termos confusos.

## Critérios de aceitação da História de Usuário
Esses critérios definem como a HU deve ser implementada, estando assim pronta quando todos os critérios forem atendidos.

### Modelo:
**Critério:** *<Descrição>*
**Dado que** *<Pré-condição>*
**Quando:** *<Ação>*
**Então:** *<Reação>*

### Aplicando os critérios de aceitação da História de Usuário

**Critério: Registro de empréstimo**
**Dado que** uma biblioteca tem o livro disponível
**Quando** informo um empréstimo a mais no sistema
**Então** o empréstimo é registrado
**E** a quantidade de livros disponíveis é atualizada