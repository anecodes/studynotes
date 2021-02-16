# Git – Conceitos Básicos

O Git é um sistema de controle de versão distribuído que foi desenvolvido com o intuito de criar um histórico de alterações durante o desenvolvimento de um software, todo em código-fonte. Além do fato de ser open-source (melhor dizendo: gratuito), outras vantagens de utilizar o Git durante o desenvolvimento de um projeto são:
* Num grupo, se uma pessoa desenvolvedora cria uma nova ferramenta no projeto **localmente**, é possível compartilhá-la através de um repositório do projeto;
* Se, no mesmo grupo, uma das pessoas desenvolvedoras perde todo o projeto local por alguma adversidade (como por exemplo algo bem comum: o HD queimou), pode-se acessar o repositório do projeto e *cloná-lo* em qualquer outra máquina;
* Durante a atualização, uma das pessoas desenvolvedoras notou que a aplicação da nova funcionalidade do projeto apresentou erros. Como o Git é baseado em sistema de versões, existe a possibilidade de "ignorar" esse erro e retornar à versão anterior do projeto.

Há também algumas outras funcionalidades pertencentes à essa ferramenta que é importante ressaltar:

## Branch

Como a própria palavra já diz, a *ramificação* é uma espécie de cópia das alterações feitas no projeto, na qual a pessoa pode alterar como quiser mas, como é uma cópia, não irá alterar o código-fonte em que está o projeto original. Desta forma, é possível alterar o projeto de forma segura, sem colocar a cópia original do projeto em perigo.

## Repositório

É o local onde o projeto será armazenado, podendo conter qualquer tipo de arquivo. Para facilitar a assimilação, é como se fossa uma "pasta" de um projeto. Pode ser armazenado localmente, utilizando apenas o Git, ou remotamente, utilizando ferramentas como GitHub, GitLab ou BitBucket.

## Merge

Caso já tenha um repositório em uma branch e alguma alteração foi feita, é hora de "dar *merge*" – ou seja, mesclar as alterações em questão com a ramificação principal do projeto.

## Fork 

Esse é um caminho inverso para a utilização de um repositório. O *fork* serve para copiar um repositório remoto (do GitHub, por exemplo) e inseri-lo em um repositório na máquina local. 

Essas funcionalidades são apenas *algumas* das inúmeras existentes no sistema de controle de versão, mas são as mais importantes. Há também os comandos principais na hora de utilizar o Git em algum projeto.

## Alguns comandos utilizados do Git

Iniciar o Git na máquina local (presume-se que o Git já está instalado na máquina em questão):
```
git init
```

Clonar um repositório (em HTTPS) remoto para a máquina local: 
```
git clone caminho/para/o/repositorio
```

Adicionar um arquivo no repositório:

```
git add . (adiciona TODOS os arquivos modificados)
```
ou
```
git add <nomedoarquivo> (adiciona um arquivo modificado por vez)
```

Descrever e confirmar mudanças feitas no repositório (também conhecido como *commitar*):
```
git commit -am "Descrição" (-a para atualizar tudo + -m para inserir a descrição)
```
ou apenas
```
git commit -m "Descrição"
```

Atualizar um repositório com a versão mais recente do projeto:

```
git pull
```

Modificar nome e email como identificação de cada commit, respectivamente:
```
git config --global user.name
git config --global user.email
```

Verificar a configuração de todas as variáveis que contém suas informações durante o uso do Git (como nome e email, por exemplo):
```
git config --list
```

Visualizar um "registro" de todas as atividades feitas no repositório do projeto:
```
git log
```

Mais informações em [Git Documentation](https://git-scm.com/docs/git/pt_BR) ou [GitHub Docs](https://docs.github.com/pt).
