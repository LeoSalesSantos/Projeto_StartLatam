####                                                     **APRESENTAÇÃO JAVAFX**

JavaFX é uma plataforma de software multimídia desenvolvida pela Sun Microsystems baseada em Java para a criação e disponibilização de Aplicação Rica para Internet, que pode ser executada em vários dispositivos diferentes.

O Java Swing faz parte do JavaSE, que roda sobre o AWT e o Java 2D. Ao passar dos anos, o Java Swing não envelheceu muito bem. Em consequência disso, foi necessário que algo novo surgisse, dando origem ao **JavaFX**, o qual utiliza conteúdo 3D, efeitos, animações, além de garantir suporte a multitouch, vídeos, áudios, etc.

**COMO INSTALAR**

Para podermos utilizar o JavaFX, precisamos adicionar ele em nossa IDE, que no nosso caso é o Eclipse.

Então vamos para o passo a passo para isso:

\1. Baixar o JavaFX

Faça o download do JavaFX. Site para download: https://gluonhq.com/products/javafx/

**Obs: nunca baixe a ultima versão pois pode ainda não ser a versão mais estável.**

Arraste a barra de rolagem e escolha a versão compatível:

 ![mat1](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat1.jpg)

\2. O segundo passo é adicionar ele ao Eclipse.

I. Vá em "Window → Preferences"

II. Na janela que se abriu vá em: "Java → Installed JREs " 

 clique no botão "Add..."

 ![mat2](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat2.jpg)

III. Em Standard VM deixe marcado e clique em "Next >"

IV. Agora Clique em "Directory..."

V. Seleciona a pasta referente ao JDK baixado.

![mat3](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat3.jpg)

VI. Depois devemos adicionar o Pacote JavaFX e para isso vá em: "Windows → Preferences"

VI. Vá em "Java" clique em "Build Path" e por fim em "User Libraries."

VII. Clique no botão "New... " Dê um nome (exemplo: JavaFX1) e clique em "OK"

![mat4](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat4.jpg)

VIII. Agora clique no botão "Add External JARs..."

IX. Vá na pasta do "JavaFX", abra a pasta "lib" e selecione todos os arquivos, exceto o src.zip.

X. Clique em "Apply and Close"

![mat5](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat5.jpg)

Caso esse processo não seja suficiente para que seja possível criar um projeto com o JavaFX, você pode seguir o processo mostrado a baixo:

\1. Abra o Eclipse e vá no menu "Help → Install New Software..."

![mat6](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat6.jpg)

\2. Em Work With coloque o seguinte endereço: https://download.eclipse.org/efxclipse/updatesreleased/2.1.0/site/

\3. Selecione "e(fx)clipse – install", depois clique em "Next >"

![mat7](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat7.jpg)

\2. Clique novamente em "Next>"

![mat8](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat8.jpg)

Para concluir necessário aceitar os termos de licença logo após clica em "Finish"

![mat9](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat9.jpg)

Pronto! Agora aguarde a instalação e a solicitação do Eclipse pedindo para ser reiniciado. Logo após, estará disponível para ser usado.

####                                         **APRENDENDO A UTILIZAR O JAVAFX**

Então vamos criar o primeiro algoritmo utilizando o JavaFX. No exemplo a seguir, faremos algo básico, usaremos a construção de interfaces de forma declarativa.

![mat10](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/mat10.jpg)

\1. Importe a classe principal herdada de (javafx.application.Application). Toda classe principal de JavaFX deve herdar de Application e implementar o método **start**;

2,No método main chamamos o método **lunch** para começar a nossa aplicação. Aqui não vai código JavaFX, o código vai no método **start**;

\3. A implementação do método **start**, herdado da classe **Application**. O atributo recebido é do tipo *Stage*. Bruscamente falando, podemos ver o Stage (palco) como o frame, a janela da nossa aplicação, mas na verdade ele não pode ser representado se pensarmos nos diversos dispositivos que podem rodar JavaFX: Celulares, televisores, "tablets", etc;

\4. Nesse ponto nós criamos um elemento chamado "pai", pois permite adicionarmos outras coisas dentro dele. No nosso caso, o StackPane permite adicionar vários elementos, os quais têm seu leiaute de pilha, ou seja, eles serão empilhados um sobre o outro. No futuro falaremos mais sobre isso, mas lembre-se que tudo no JavaFX é um nó, ou seja, herda da classe Node;

\5. Não há nada demais aqui, simplesmente criamos um objeto do tipo Label, que é um controle de interface para mostrar texto;

\6. Aqui informamos o texto que o Label irá mostrar. Note que isso poderia ter sido feito pelo construtor, na criação do Label;

\7. Como o StackPane é um elemento pai, ele também tem elementos filhos. Nessa linha de código, recuperamos os filhos dele **(getChildren())** e adicionamos nosso Label **(add(Node)),** fazendo que o Label seja um filho dele;

\8. É hora de aprender outro conceito do JavaFX. Nessa linha criamos uma Scene (cena). Uma cena é o container principal de todos os elementos do JavaFX e na criação dela aproveitamos para informar a raiz (como o nome diz, a raiz de todos os componentes), largura e altura da cena;

\9. Agora vamos voltar a mexer com nosso palco. Nessa linha informamos o título dele, no nosso caso atual, o título da janela que será mostrada;

10.O palco precisa de uma cena, simplesmente é isso que é feito nessa linha.

11.Simplesmente mostrando o palco! Se esse método não for chamado, nada irá acontecer quando executar esse código.

**IMPLEMENTAÇÕES DO JAVAFX**

O JavaFX é uma ferramenta que expande o poder do Java, permitindo que usuários da linguagem possam usar qualquer biblioteca Java nas aplicações JavaFX.

Assim, os usuarios podem expandir ainda mais seus recursos no Java aproveitando a tecnologia de apresentação que o JavaFX fornece para criar experiências visuais envolventes.

Os Sites abaixo possui outros exemplos interessantes que possam implementar nos futuros projetos de vocês:

} https://code.makery.ch/blog/javafx-8-event-handlingexamples/

} http://aprendendo-javafx.blogspot.com/p/o-que-ejavafx.html

} https://github.com/dlsc-software-consultinggmbh/FormsFX

} https://openjfx.io/



Autor: Matheus Henrique
