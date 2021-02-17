# Introdução à Linguagem C

## Abstração
É a característica de se concentrar em aspectos essenciais de um conceito, ignorando os demais detalhes menos relevantes.
Em Orientação a Objetos, uma classe é chamada de uma abstração de várias entidades que existem em um mesmo sistema.

## Estrutura de um programa em C

```
#include <stdio.h>
#define MAX_NUM = 15

int vlglobal = 10; //Declaração de variáveis globais

int main (int argc, char *argv[]) //Início de qualquer aplicação C
{
    int i, j, ncols; //Declaração de variáveis locais
    
    for (i=1, j=1 ; i<=MAX_NUM ; i++, j++) //Comandos e expressões
    {
        printf("%2d",i);
        if (j == ncols)
        {
            j=0;                //Outras funções
            ncols++;
            printf("\n");
        }
    }
}
```
## Diretivas de compilação
*  #include: incorpora definições de funções, declarações de tipos de dados e estruturas, além de constantes, que são colocados em arquivos de cabeçalho (header = h).
Cabeçalhos da biblioteca padrão:
- stdio.h: funções de input/output
- stdlib.h: funções complementares
- string.h: funções de string
- math.h: funções matemáticas

* #define: permite declarar constantes que poderão ser substituídas no código pelo pré-compilador.

## Variáveis em C
* **Modificador da classe de armazenamento:** auto, extern, register, static;
* **Modificador de acesso:** const, volatile;
* **Modificador de tipo:** short, long, signed, unsigned (esses modificadores podem ser combinados!);
* **Tipo:** char, int, float, double, void.

## Estruturas de controle de fluxo de execução

* **Comando de comparação ou seleção:**
 - If/else:
 - 
```
if (expressão 1)
    //comando 1
   else
    //comando 2
````
ou
``` 
if (expressão 1)
    // comando 1
    else
     if (expressão 2)
    // comando 2
    else
     if (expressão 3)
    // comando 3
    else
    // comando 4
``` 

- While/do:

```
while (expressão 1)
 //comando 1
``` 
ou

```
do {
// comando 1
} while (expressão 1);
```

- For:
```
for (atribuição ; expressão 1 ; incremento)
// comando 1
``` 
## Vetores
 - Dados homogêneos, ou seja, têm o mesmo tipo;
 - Os elementos de um vetor são identificados pela sua posição dentro deste, o qual é chamado de "índice";
 - Em C, o primeiro elemento do vetor é sempre rotulado com o índice ZERO (0);
 - Partindo disso, é certo indexar o último elemento por "n-1", sendo n o tamanho do vetor.

## Funções e declaração de funções

### Formato:

```
retorno_tipo nome_da_funcao (parâmetros); |
{ corpo da função }
```

- Em C, rotinas e funções não possuem diferenciação, e funções com retorno *void* são também consideradas rotinas;
- Para ser chamada no corpo do código, a função deve ser declarada no ínicio do programa, após as diretivas de pré-compilação;
- Para chamar a função, faça da seguinte forma no trecho do programa que gostaria de referenciá-la:
```
nome_da_funcao (lista de parâmetros);
``` 
### Passagem de parâmetros

```
void func1 (int par1, char par2, const char par3[])
```
- Para que o conteúdo do parâmetro não seja modificado, o correto é utilizar o modificador *const*;
- Para realizar a passagem de parâmetros por referência, usa-se *ponteiros*.
- Como não é possível passar matrizes com as duas dimensões desconhecidas, utiliza-se o * *argv[]* em main, no qual o * representa um ponteiro e uma das dimensões.
