## Introdução à Análise Orientada a Objetos (AOO)

É um paradigma entre AOO, Projeto Orientado ao Objeto e Linguagem de Programação que se baseia em unidades de software, chamadas de **objetos**. A AOO tem como objetivo encontrar a melhor maneira de descrever um sistema de software através de objetos e funciona através de troca de mensagens entre esses objetos.

**Alguns conceitos:**

**Classe:** conjunto de objetos que possuem características em comum. A classe define o comportamento dos objetos através dos métodos, e também quais estados pode manter através dos atributos. Exemplo de classe:

```CACHORRO é uma classe e tem como atributos: 4 PATAS, 2 OLHOS, 1 FOCINHO, etc.```


**Objeto:** instância da classe, junção dos conceitos *dado* + *operações*. Exemplo de objeto da classe CACHORRO:

```CARAMELO é um objeto da classe CACHORRO, e apresenta todos os atributos dessa classe, mas com suas próprias características```

**Herança:** quando uma subclasse pode se prolongar a outra classe, usando os mesmos métodos e atributos. Há herança múltipla quando uma subclasse tem mais de uma superclasse. Exemplo de herança:

```ANIMAL é superclasse de CACHORRO. Sendo assim, um cachorro é um animal.```


## UML (Unified Modeling Language)

É uma linguagem para especificação, visualização e documentação de artefatos de sistemas de software que utilizam Análise Orientada a Objetos. É a norma da indústra para a produção de software.
A UML (ou Linguagem de Modelagem Unificada) **não é uma metodologia**, mas sim uma notação para a AOO.


### Por que utilizar UML?
* Porque pode ser utilizada em todas as fases de análise, projeto e implementação;
* Trabalha com diversos diagramas e artefatos com uma noção clara e consistente;
* Não se prende a uma só metodologia, sendo que todas podem utilizar a UML;
* Facilita o entendimento entre o cliente e a área de TI.

### Tipos de artefatos UML:
* Diagrama de Caso de Uso
* Especificação de Caso de Uso
* Diagrama de Classes
* Diagrama de Objetos
* Diagrama de Sequência
* Diagrama de Atividades
* Diagrama de Transição de Estados

### Caso de Uso

O Caso de Uso é um detalhamento de requisitos. É possível que um requisito gere um ou mais caso de uso. 

Normalmente, **um** caso de uso se torna **uma** tela. Não é uma regra, mas é comum acontecer.

## Diagrama de Caso de Uso
Um diagrama de Caso de Uso serve para mostrar graficamente os Requisitos do sistema, as interações entre elas e com entidades externas.

### Alguns conceitos:

Elementos do diagrama: 
* Ator
* Caso de Uso
* Relacionamentos

**Ator**

O ator é alguém ou algo que interage com o sistema, que utiliza o sistema.

Tipos de atores:
* Pessoas
* Órgãos de uma organização
* Outros sistemas informatizados

**Caso de uso**

Um caso de uso é uma funcionalidade completa do sistema, após o ator interagir com a mesma. Além disso, o caso de uso também descreve o ator na intenção de realizar uma ação no sistema e também fornece um resultado ao ator.

**Relacionamentos**

* **Relacionamento entre Ator e Caso de Uso**
Mostra que há uma interação entre o Ator e o Caso de Uso, ou seja, o ator está recebendo ou entregando informações do Caso de Uso.

* **Relacionamento entre Atores – Herança**
Os atores podem ser configurados através de hierarquias, nos quais atores com maior complexidade herdam comportamentos de atores mais generalizados.

* **Relacionamento entre Casos de Uso – Herança**
É utilizado quando um Caso de Uso possui semelhança com outro, porém tem um pouco mais de complexidade. Sendo assim, é certo afirmar que o segundo caso é uma especialização do primeiro.

* **Relacionamento entre Casos de Uso – Include**
Acontece quando há uma parte do comportamento do Caso de Uso que pode ser utilizada em outro caso. Esse tipo de relacionamento evita repetições, visto que apenas é necessário fazer um caso e utiliza-se esse caso.

* **Relacionamento entre Casos de Uso – Extend**
Possui semelhança ao Include, porém só existe quando acontece uma determinada condição, ou seja, somente se essa condição for verdadeira.




