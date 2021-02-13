# Diagrama de Classes

## Objeto

É algo existente, seja ele concreto ou abstrato, que possui:
* Atributos;
* Identidade (sendo este o **nome** do objeto; cada objeto é único);
* Comportamentos.

### Atributos:

Características dos objetos, tais como:

Nome do doce: Dorayaki
Do que é feito: ovos, manteiga, açúcar, farinha de trigo, fermento em pó, mel, molho de soja
Origem: Japão

### Comportamentos (ou Operações/Métodos/Funções):

Ações feitas pelos objetos, ou seja, é como os objetos reagem a outro objeto.

Exemplo de comportamento do objeto Bolo: inserirRecheio

## Classe

Conjunto (ou coleção) de objetos que possuem a mesma lista de atributos e comportamentos, assim como o mesmo relacionamento com outros objetos. Uma classe pode ser usada como referência para obter objetos com características similares. A classe é como um protótipo que define variáveis e métodos de mesmo uso por todos os objetos de uma classe.


## Outros conceitos relevantes que descrevem a CLASSE:

* São objetos que obedecem a uma mesma especificação;
* Um objeto também pode ser chamado de Instância de Classe.


### Encapsulamento
As atribuições e as operações de cada objeto estão armazenados nele mesmo, ou seja, encapsulados no objeto. A função desse encapsulamento é de evitar o acesso desordenado dos dados. Nesta modalidade, o acesso só é possível através de operações executadas entre os objetos.
           
**!** Os nomes das *classes* devem ser escritas no singular, sem caracteres especiais, traços ou espaços, sem preposições e devem ser escritas com a primeira letra da palavra maiúscula e as demais, minúsculas. Exemplo: **PessoaFisica**, **CaixaEstoque**, etc.

**!** Os nomes dos *atributos* devem ser escritos sem caracteres especiais, traçosou espaços, sem preposições e devem ser escritos em camel case. Exemplo: **numeroCaixa**, **idadeAluno**, etc.

## Diagrama de Classes

O diagrama de classes mostra as classes e os relacionamentos entre elas em um sistema. A classe é representada por uma caixa, dividida em três partes com identificação, atributos e métodos. Exemplo:

| Classe |
----------
| atributo1: int | 
| atributo2: int |
| metodo1(): void |
| metodo2(): void|


### Relacionamentos

Os objetos também podem ter algum tipo de relacionamento entre si, como as Associações, as Agregações, as Composições e a Herança

### Associações

Representam uma conexão entre dois elementos de uma classe, no qual tal relacionamento só existe se houver alguma referência de um ao outro.

**Cardinalidade ou multiplicidade das associações:**

* Muitos: *
* Exatamente um: 1
* Zero ou mais: 0 .. *
* Um ou mais: 1 .. *
* Zero ou um: 0 .. 1
* Intervalo específico: 2 .. 7

### Agregações

É uma associação na qual o elemento que está associado representa uma parte do elemento principal. Exemplo: 

**Música** ----<> **Playlist**
**Açúcar** ----<> **Bolo**

### Composições

É um modo de agregação na qual as partes pertencem apenas a um todo preestabelecido. Neste caso da composição, não há lógica obter o objeto da classe principal sem seus objetos. Exemplo:

**Caderno <>**---- **Folha**
**Flor <>**---- **Buquê**

### Herança
É quando um objeto-filho "herda" características e comportamentos de um objeto-pai, que já existe. Dessa forma, é possível que novas classes possam tomar propriedades de classes-mãe e também incluir novas características.

Exemplo:

Classe Pai | Atributos
---------- | ----------
Cliente    | telefone