####                                                                  **Array**

Array ,em português "vetor", é o responsável pelo armazenamento de mais de uma variável, ou seja, é quem permite que diversos valores possam ser guardados sem que tivéssemos que criar inúmeras variáveis.

Os vetores são indicados de acordo com a seguinte sintaxe:

**tipo[ ]** *nome_vetor* = new **tipo** [tamanho_vetor];

obs: o tamanho do vetor começa na posição 0. Ou seja, se um vetor possui 2 dados armazenados nele, esses dados estarão alocados na posição 0 e na posição 1.  Além disso, é importante destacar que os vetores só podem ter tamanhos do tipo **int**, e nunca double, byte, short, etc. 

**dica:** quando você quiser percorrer todo um vetor dentro de um ciclo for por exemplo, ao invés de colocar o tamanho do vetor para ser corrido, coloque apenas o comando *length*.

**Exemplo:**

Scanner teclado = new Scanner(System.in);

**int[ ]** idades = new **int** [3];

for (int i=0; i<3; ++i){  //o ciclo deve começar com i=0 porque o vetor começa na posição 0
          System.out.println("Digite a idade:");

​    idades [i]= teclado.nextInt();

​    }



  **OU**

Scanner teclado = new Scanner(System.in);

**int[ ]** idades = new **int** [3];

for (int i=0; i<**idades.length**; ++i){  //o ciclo deve começar com i=0 porque o vetor começa na posição 0
          System.out.println("Digite a idade:");

​    idades [i]= teclado.nextInt();

​    }

**Características:**
.Um array pode ter uma ou diversas dimensões. As dimensões constituem os locais onde nossos
valores serão armazenados.
.Todo Array possui um índice e este representa um único elemento do Array.
.Elemento é o nome de cada item do nosso Array. Assim, todo Array irá possuir no mínimo um item em
cada dimensão.

**Collections**
As collections, em português "coleções", são os conjuntos de interfaces e de classes que servem para
representar/armazenar vários grupos de dados. Com isso, torna-se possível armazenar e ler dados sem a
necessidade de sabermos como esses dados serão armazenados, dando origem assim ao encapsulamento.

**São as interfaces :**
.List
.Set
.Queue
.Deque
.Sortedeset

**São as classes :**
.Arraylist
.Linkedlist
.Vector
.HashSet
.PriorityQueue
.LinkedHashSet
.TreeSet

####                                                                   **Listas**

O List é uma interface, enquanto que o Arraylist é a classe que a implementa. Uma Arraylist pode representar vários objetos de tamanhos e formas variadas, podendo assim ter um tamanho que infinito. Já os Arrays possuem tamanho fixo, previamente determinado pelo programador.

**Sintaxe**: List< tipo > nome_ArrayLIst =  new ArrayList < tipo >();

obs: O tipo da variável nesse caso deve vir com letra maiúscula, ex: **String** (e o tipo inteiro ao invés de **Int** deve ser **Integer**). Além disso, lembre-se de importar: *import java.util.List* e  *import java.util.ArrayList*.

**Métodos da classe List:**
**.**add – Adiciona um item no final da coleção;
.get – retorna (pega) um item em determinada posição;
.set –altera o valor de um item em uma determinada posição;
.size – retorna o tamanho atual da coleção;
.clone – duplica a ArrayList;
.contains – busca um valor no array, e retorna "true" se o elemento estiver no array;
indexOf - ele busca um valor no array, mas retorna o índice do elemento encontrado ou em LastIndexOfo mesmo que indexOf mas retorna o último elemento encontrado;
.remove – remove um item da coleção.

**Exemplo:**

List< String > nomeAlunos =  new ArrayList < String > ();

nomeAlunos.add ("Pedro");

nomeAlunos.add ("Paula");

System.out.println("Confira os nomes:");

for (int i=0; i< nomeAlunos.size(); ++i){ /*você pode digitar 2 ao invés de nomeAlunos.size(), já que são 2 nomes (esse comando do size é similar ao **length** usado nos vetores) */

System.out.println("-" + nomeAlunos.get(i) ); /* esse get vai resgatar o nome digitado na posição i. Ou seja, quando i for igual a 0, o programa vai procurar qual nome foi atribuido à posição 0 do ArrayList (que no caso é o nome Pedro). Ademais, esse "-" foi digitado só para os nomes saírem listados assim: 

-Pedro

-Paula

*/

}



Autora: Maria Eduarda Theodoro