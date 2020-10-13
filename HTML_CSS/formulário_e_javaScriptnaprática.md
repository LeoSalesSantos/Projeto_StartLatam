####                                                                                                         **Formulários**

Os formulários são a forma que usamos para o usuário interagir com web site, podendo
enviar dados que são enviados para um servidor web. Um exemplo que podemos dar
de interatividade com o usuário é um cadastro de um web site.

NOME:&lt;input type=”text” size=”20” maxlength=”45” name=”nome”/&gt;

 EMAIL:&lt;input type=”text” size=”20” maxlength=”45” name=”email”/&gt;

SENHA:&lt;input type=”password” size=”20” maxlength=”45” name=”senha”/&gt;
         &lt;input type=”submit” value=”ENVIAR”/&gt;

![lari20](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_HTMLCSS/lari20.PNG)

Os elementos de um formulário variam de acordo com o tipo de informação que será
inserida. Exemplo: text, password, checkbox, file, radio entre outros.

**Atributos**
*Action:* usamos action para fazer a execução da ação quando clicamos para enviar as
informações inseridas.
*Method:* defini qual método usamos para enviar o formulário, usando get para
recuperar informações do servidor e limitar a quantidade de dados a serem enviado e,
o post para inserir as informações sem limitar a quantidade de dados.
*Name e Id:* esses atributos podem ser usados em qualquer elemento do html e,
funcionam como nomeadores do elemento para identificação.

####                                                   **JavaScript**

Com essa linguagem muito popular podemos implementar funcionalidades mais complexas, deixando a página web mais dinâmica. O código deve ser usado junto com os comandos HTML, visto que ele permite executar instruções conforme a resposta das ações do usuário, podendo criar assim uma calculadora, por exemplo.

**Exemplo de JavaScript:**

< html >

< head > < title > Minha página JavaScript < /title > < /head >

< body >

< h1 > Página oficial do GSCursos < /h1 >

< script type = "text/ javascript" > document.write ("Bem vindo ao GSCursos");

< /script >

< /body >

< /html >

​                                               

####                                                                  **JavaScript**

O JavaScript é uma ferramenta bem útil para um programador em seu trabalho ou para iniciantes e podemos trabalhar em diversas formas com ele. Vamos ver alguns exemplos de como podemos trabalhar em JavaScript. 

**Exemplo:**

![lilian20](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_HTMLCSS/lilian20.PNG)



O JavaScript é uma ferramenta que você consegue mostrar mensagens e outras informações, fazer verificações e executar a página de forma que você programou. Isso tudo através do nosso próprio aplicativo.

**Como programar em JS?**

Usando variáveis, e iremos ver como podemos usá-las:

·     var nome = "Ana Maria";

·     var idade = 25;

   

Da mesma forma que aprendemos no Portugol, em JS também especificamos o seu tipo. Se é: inteiro, real e entre outros. Podemos somar ‘A’+‘C’ em JS, pois um número decimal da mesma forma que um inteiro, mais abaixo veremos exemplos.

 

**Características do JS:**

·     Fornece suporte a funções.

·     As funções podem receber parâmetros e retornar valores(os parâmetros não precisam ter um valor imutável).

 

**Exemplos de Funções com parâmetros de retorno:**

 

function exibirMensagem () {

alert(“Bem Vindo(a), caro Aluno(a)!”);

}

 

**Exemplos de Funções sem parâmetros de retorno:**

function somar (A, B) {

return A + B;

}



![lilian21](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_HTMLCSS/lilian21.PNG)





![lilian22](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_HTMLCSS/lilian22.PNG)





**Unindo HTML, CSS e JS**

Arquivo HTML
                                        

< !DOCTYPE html >

< html >

< head >

< title >Unindo HTML, CSS e JS< /title >

<script type="text/javascript" src="js/nomeArquivoJavaScript.js"></script>

< script src="aula8.js">< /script >

< meta charset="UTF-8" >

< /head >

< body >

< h3 >Unindo HTML, CSS e JS< /h3 >

<p id="p1">Selecione:</p>

<button onclick="clique_botao1();">Opção 1</button>

<button onclick="clique_botao2();">Opção 2</button>

< /body >

< /html >

 

  Arquivo JS

 

functionclique_botao1() {

​        document.getElementById("p1").style.color="red";

}

functionclique_botao2() {

document.getElementById("p1").style.color="blue";

}



Autora: Larissa Caroline e Lilian Ribeiro



