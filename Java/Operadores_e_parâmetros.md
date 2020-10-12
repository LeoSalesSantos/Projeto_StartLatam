####                         **Ambiente de desenvolvimento integrado (IDE)**

IDE é um software que auxilia no desenvolvimento de aplicações, muito utilizado por
desenvolvedores, com o objetivo de facilitar diversos processos durante o desenvolvimento de
aplicações, que combinam ferramentas comuns em uma única interface gráfica ,que é o caso do
Eclipse.

**Regras para declaração de uma variável**
. para identificar uma variável é possível utilizar letras maiúsculas e minúsculas, números ou caracteres
de sublinhado _
. Porém não pode utilizar como nome uma palavra reservada nem começar por um número.

Sintaxe: tipo identificador;

* **Exemplos:**

String nomeComoleto;

Char letra;

Int idade;

Float total1;total2;total3;

Byte v;

Boolean confirmar;

Double valorMedio;

. Obs: String é o único apresentado aqui que não é um tipo primitivo. Ele é um tipo objeto pertencente a classe interna do Java pacote Java .Lang, por isso é o único escrito com inicial maiúscula.

**Conversão de identificadores (nomes)**
Não é obrigatório, porém existe a conversão padrão para atribuir nomes em Java.

. Classes devem sempre ser indicados por letras maiúsculas;

*Exemplo: Pessoa, Conta

. Métodos ,atributos ,variáveis ,objetos seguem a seguinte regra;

. Apenas um nome, o qual inicia-se por letras minúsculas

*Exemplo: calcular(),pessoa,aluno

. nome composto, primeira palavra com letra minúscula e a segunda com letra maiúscula

*Exemplo: calcularTotal(), calcularMedia(),

Obs: lembre-se de seguir a conversão CamelCase, a qual é uma conversão legalmente aceita que alega que devemos começar os nomes com letras minúsculas e, a cada nova palavra, começá-la com maiúscula.

*Exemplos: nomeDeVariavel

nomeDeAtributo

nomeDeMetodo

NomeDeClasse

**Atribuição de valores em variáveis:**

Operador de atribuição: =

:arrow_right: Atribuindo valores:

nome="João";

idade=25 ;

altura=1.85;

peso=60.5f;

ativo=true;                                         


:arrow_right: Declaração e atribuição:

String nome="João";

Int idade=25 ;

double altura=1.85;

float peso=60.5f;

boolean ativo=true;

*Obs: não confunda um operador de atribuição (=) com um operador de igualdade (==)

Principais tipos de variáveis:

**Inteiros:**

int (inteiro)

byte(inteiro curto)

short (inteiro médio)

long (inteiro longo)

**Ponto flutuante (números reais):**

float (ponto flutuante simples)

double (ponto flutuante duplo)

**Lógico:**

boolean (lógico: true, false)

**Char**

O tipo char permite a apresentação de caracteres individuais. Geralmente utilizados para armazenar o
caractere da tabela ASCI, e sempre delimitada por apóstrofos. 

*Exemplo:

char sexo = 'M'

**Tipo objeto: String**

É um objeto do Java que armazena valores que são uma sequência de caracteres do tipo char. Uma String é sempre delimitada por aspas.

*Exemplo:

String apelido ="jo";

String nomeCompleto="joão roberto da silva";



**Como usar as classes**

Usa-se o comando *import*, que serve para identificar e carregar classes de nossa escolha. As instruções *import* devem aparecer antes da definição das classes.

*Exemplo: import Java.util.Scanner;



**Classes pré-definidas no JDK**
A biblioteca é formada por conjunto de classes do jdk que são organizadas em pacotes. Alguns exemplos delas são:
. Java. Lag: funcionalidades básicas da linguagem, costuma ser importado automaticamente em seus
programas Java e ainda inclui as classes String, Math, Integre , Thread, entre outras

. Java.awt: componentes gráficos originais da linguagem (Abstract Window Toolkit)

. Java.swing: pacote de extensão aos componentes gráficos com melhoramento a biblioteca AWT

. Java.applet: classes específicas para tratamento de applets

. Java.net: recursos de rede (sochets e URLs)

. Java.io: classes para escrita e leitura em arquivos

. Java.util: classes para tarefa gerais tais como vetores e strings de tokens.

**Um pacote especial**

Java.lang.*( dispensa import)

. A classe system

Possui os métodos out.print(),out.println(), o que é o comando de saída de dados mais básico do Java

. A classe String

É uma classe especial que representa o tipo caracter. Mas além dela há outros tipos de classes que representam os tipos primitivos que são chamadas de
"classes Wrapp".



####                                              **Entrada e saída de dados**

                                       	Portugol                                     Java
                                        escreva()                              System.out.print();
                                        escreval()                             System.out.println();

Existe uma diferença entre "print" e "println", visto que esse comando "In" faz com que, após a impressão do dado, o cursor continue o programa na linha seguinte.

Ao utilizar métodos de saída de dados podemos utilizar conjunto de algumas sequências de escape (funções de barra invertida), como: 

**\n:** nova linha - posiciona o cursor no início da próxima linha.

**\t:** tabulação horizontal - move o cursor para a próxima parada de tabulação.

**\r :**coloca o curso no iníco da linha atual, não avança para a próxima linha.

**\\:** Barras invertidas. Usada para imprimir um caractere de de barra invertida

**\": **Aspas duplas. Usada para imprimir um caracter de aspas duplas (coloque \ antes da ")

*Exemplo de aspas duplas:  System.out.println("\\"aspas\\""); exibe "aspas"

**Printf**

É um método que corresponde a uma String de formato, que pode ter como intuito texto fixo e especificadores de formato. A letra "f" no final da palavra print significa "formatted", a qual faz com que exiba dados formatados.

*Exemplo:
public class Texto_printf{
public static void main (String [ ] args){
System.out.printf ("%s\n%s\n", "Luciana", "Silva");
}
}

                                        Portugol                                     Java
                                         Leia()                         Scanner ler=New Scanner (System.in)
                                                                                  n=ler.nextIn;()

Resumidamente, para utilizarmos um método de entrada de dados temos que seguir as seguintes orientações:
        1- Importar o pacote Java util
Ex: Import.java.util.Scanner

2- Instanciar um objeto Scanner
Ex: Scanner ler=New Scanner (System.in)

3-ler através do teclado (exemplo: uma variável n do tipo inteiro);
Ex: System.out.printf("informe um número para a tabuada: ")
n=ler.nextInt();



#### **Métodos**

. Os métodos realizam tarefas, tais como cálculos e comunicação com outros objetos;
. Processam sobre variáveis/atributos de classes ou objetos, alterando o estado atual do programa;
. Em Java, métodos são similares às funções, sendo assim podem apenas executar uma tarefa ou também retornar um valor qualquer para o trecho do programa que o invocou (chamando o método).

Declaração de métodos:
Caso quisermos separar as instruções do programa em partes menores para que possamos modificá-las mais facilmente, devemos criar vários métodos.

####  **Operadores Aritméticos:**

Conjunto de símbolos que representam operações básicas de matemática

Adição: +

Subtração: -

Multiplicação: *

Divisão: /

Resto da divisão: % (não é o mesmo que porcentagem)

#### **Operadores Relacionais:**

Utilizados para comparar valores


Maior que: >

Menor que: <

Igualdade: ==

Maior ou igual: >=

Menor ou igual: <=

Diferente de: !=

#### **Operadores Lógicos:**

Também são utilizados para comparar valores, porém a diferença está na forma com que os operadores avaliam seus operandos. Esta avaliação resulta em verdadeiro e falso.

&& (E)    O resultado será verdadeiro somente se todos os valores da comparação forem verdadeiros

|| (OU)  O resultado será verdadeiro somente se pelo menos um dos valores da comparação for verdadeiro (todos não podem ser verdadeiros aqui)

! (NÃO) O resultado será verdadeiro somente se a expressão for falsa.

Um pouco mais sobre métodos..
Os métodos também possuem um tipo de identificador (nome). Ademais, eles recebem parênteses ( ), que podem ou não ter a declaração de parâmetros. Além disso, nos métodos também há uma implementação de chaves { }, exceto para métodos abstratos.

#### **Parâmetros:**

São valores passados pelos métodos para que possam ter às instruções realizadas naquele método.
*Exemplo:

 Double soma (doublen1, doublen2){

return n1+n2

 }

**Retorno:**
        O comando "return" retorna o valor calculado naquele método com base nos parâmetros digitados (caso existam). No exemplo anterior, o valor que será retornado para o método principal será a soma de n1 com n2. 

Os métodos podem retornar o valor de uma variável. O tipo de retorno é definido antes do nome do método.
*Obs: void indica a ausência de um tipo de dado. O método que declaramos como void não retorna
valor algum (ou seja, se criarmos um método do tipo void, ele não poderá ter o comando "return").

**Modificadores de acesso:**
São palavras-chaves que garantem níveis de acesso a atributos, métodos, classes e padrões de
visibilidade.
São exemplos de modificadores de acesso: Public ,Private,Protected,Defalt,final,Abstract e Static



Autora: Maria Eduarda Theodora
