####                                            **Getters e Setters**  

São métodos usados em classes sempre que realizamos um encapsulamento (realizar limites ao acesso a atributos de uma classe exclusivamente através dos métodos. Os limitadores de acesso são: public, protected e private). E esses atributos só poderão ser usadas em outras classes através desse métodos.

:arrow_right: Public: Permite acesso a qualquer código externo.

:arrow_right: Protected: Permite acesso as classes filhas, mas proíbe qualquer excesso externo.

:arrow_right: Private: Proíbe acesso as classes filhas e a classe principal.

Sendo assim, para conseguir permitir o acesso (nas classes privates), é interessante criar
os dois métodos (get e set), já que um retorna e o outro muda o valor.

**Exemplo usando método get e set no código:**

public class Pessoa {
private String nome;
public String getNome() { //sempre retorna um valor, obtém informações
return this.nome; //
}
public void setNome (String nome) { //define valores, não retorna
this.nome=nome;
}

####                                               **Erros e exceções:**

Exceções: Ocorrem quando algo imprevisto acontece.

**Ex de motivos externos:** tentar abrir um arquivo que não existe, tentar conectar em
algum servidor inexistente, etc.

**Ex de motivos de lógica:** tentar manipular um tipo de dado como se fosse outro, dividir
um núero por 0, etc.

E geralmente o código não consegue ser executado. O uso das exceções é muito
importante pois pode evitar e tratar futuros erros. E existem 2 tipos:

**Implícitas=** não precisam de tratamento e demonstram serem contornáveis. Esse tipo
origina-se da subclasse Error ou RunTimeException.

**Explícitas=** Precisam ser tratadas e apresentam situações incontornáveis, esse tipo
origina do modelo throwe necessita ser declarado pelos métodos. É originado da
subclasse Exception ou IOException.

**Existe também a formação de erros tipos throwables:**

Checked Exception= acontecem fora do controle do programa, mas que devem ser
tratados pelo desenvolvedor para o programa funcionar.

Unchecked(Runtime)= podem ser evitados se forem tratados e analisados pelo
desenvolvedor.

Error= para indicar um problema do programa, tornando impossível a execução.

:arrow_right: O erro é algo que não pode ser mais tratado, já as exceções conseguimos reverter os
problemas e executar o código.

####                                         **Try, catch e finally:**

Criados para tratar exceções, tem o objetivo de impedir erros e ele mesmo determina o
que fazer com as exceções.

O bloco **try** tem a função de executar o código que estiver dentro das chaves, isso seria a
mesma coisa que dizer: “o código que está dentro desse bloco pode gerar exceções”.

O bloco **catch** tem a função de tratar a exceção lançada no try, dependendo do tipo que
for, o sistema para e lança a exceção do erro.

Já o bloco **finally** é opcional, e tem a função de finalizar a sequência de comandos.

:arrow_right: Basicamente o uso de exceções é relacionado a códigos que pedem interação com os
dados, ou seja, tudo que apresentar algum risco necessita do tratamento dos
erros.

:arrow_right: A classe Throwable inclui o registro do estado atual da pilha chamada de método e
uma String associada a uma mensagem de erro, que pode ser obtida para qualquer
exceção através do método Throwable.getMessage().

####                    **API JAVA (Application Programming Interface) **

 É a interface normalmente documentada que uma biblioteca ou framework disponibiliza para que o programador possa utilizá-la. E elas podem ser:

:arrow_right: **Públicas=** disponibilizadas de forma gratuita e são utilizadas, por exemplo, em redes
sociais.

:arrow_right: **Privadas=** Requerem login e senha e normalmente são pagas.
Alguns exemplos de APIs são: Google Maps, Paypal, Facebook, etc.
Essa interface permite que as mais variadas funções de um determinado site possam ser
utilizadas em uma outra plataforma, e oferece uma rica coleção de classes e métodos
para realizar cálculos, manipular Strings, verificação de erros, etc.

:arrow_right: Uma API pode oferecer uma série de vantagens, como: facilidade, segurança de
dados, controle de acessos, etc.
**JSP (Java Server Pages) =** As páginas JSP estão compostas de códigos em HTML. Elas são
arquivos de texto com a extensão .jsp. , e necessitam de um servidor para funcionar, como
o Tomcat (um servidor disponível gratuitamente). Para conseguir ter HTML e JAVA,
utilizamos o comando &lt;% %&gt; para escrever o código em Java (e o restante escrevemos com tags HTML).
**JDBC (Java Database Connectivity) =** É uma API que conecta conjuntos de classes e
interfaces escritas na linguagem Java, na qual possibilita o uso do banco de dados (SQL).



Autora: Anna Beatriz
