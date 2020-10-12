####                           **FRONT-END E BACK-END**

:arrow_right: **Front-end:** O desenvolvedor front-end, fica responsável pela parte
visual de um site, ele cria através de um código, uma inteface gráfica
que irá rodar no navegador. As ferramentas utilizadas são: HTML, CSS
e Javascript.

:arrow_right: **Back-end:** O desenvolvedor back-end, trabalha de forma oculta, onde o
usuário não possa manipular algo ou ter acesso. Toda parte envolvendo
entrada de informações para um banco de dados, são os back’s que
fazem essa programação. Há diversas linguagens que fazem essas
programações, entre elas: PHP, Java, C# e Ruby.
HTML(HyperText Markup Language)

:arrow_right: É uma linguagem usada pelos desenvolvedores Front-end, para
determinar como será exibido um documento. Um programa muito
usado para construir um arquivo HTML, é o Notepad++. Existem outros
como o VisualG.

:arrow_right: É dividido em três partes: estrutura principal, cabeçalho e corpo de texto.
TAGS

:arrow_right: As TAGS são comandos de formatação, que possibilitam fazer as
criações e edições para o site.

:arrow_right: Para iniciar uma TAG, usamos &lt;&gt;. E para fechar usamos &lt;/&gt;.
Lembrando que a TAG tem que estar dentro, como no exemplo: &lt;title&gt;
&lt;/title&gt;.

**Funções de algumas TAGs:**
&lt;html&gt;: Inicializa e finaliza todo o projeto, é a primeira TAG a ser inserida;
&lt;head&gt;: Delimita o cabeçalho;
&lt;title&gt;: Título do elemento, exibido na barra do site;
&lt;body&gt;: Tudo que será exibido no site deverá estar no body;
&lt;p&gt;: Parágrafo;

&lt;font&gt;: Fonte da letra;
&lt;br&gt;: Quebra de linha;
&lt;align&gt;: Alinhamento (center,right,left e justify);
&lt;width&gt;: Largura;
&lt;height&gt;: Altura;

**META TAG**

:arrow_right: A Meta TAG descreve o conteúdo do site, passando informações
importantes para os navegadores. É importante inserirmos no inicio do
documento HTML, dentro do &lt;head&gt;&lt;/head&gt;.
Charset&lt;meta charset=”UTF-8”&gt;

:arrow_right: Essa Meta TAG permitirá a utilização de caracteres, como ~, ´,^ e que
sejam exibidos de forma correta, sem a quebra dos mesmos.

**COMENTÁRIOS**

:arrow_right: Os comentários, são breves anotações que o criador acha relevante
guardar, para ter controle do que está sendo feito. Lembrando que todo
conteúdo comentado, não será exibido no site.
Sintaxe do comentário: &lt;!-- Comentário --&gt;

**TABULAÇÃO**

:arrow_right: Formatação do código, para facilitar o entendimento dos
desenvolvedores do projeto.

**TÍTULOS E SUBTÍTULOS**

:arrow_right: Para formatar o tamanho de títulos e subtítulos, usamos as tags
heading (h1 – h6).

:arrow_right: O &lt;h1&gt;&lt;/h1&gt; é o tamanho maior (primeiro nível), a partir desse, as letras
vão diminuindo.

**ALINHAMENTO DE TÍTULOS**

:arrow_right: Existem quatro formas de fazer seu alinhamento, utilize o parâmetro
align e acrescente a propriedade que desejar.
o Center (centro)
o Right (direita)
o Left (esquerda)
o Justify (justificado)

 Exemplo: &lt;h2 align=”justify”&gt; Teste &lt;/h2&gt;;

**LISTAS**

:arrow_right: Não ordenada: Utiliza-se a TAG &lt;UL&gt;&lt;/UL&gt; e &lt;LI&gt;&lt;/LI&gt;.
o Circle (Lista com círculo)
o Square (Lista com quadrado)
o Disc (Lista com disco)
 Sintaxe: &lt;UL TYPE=”circle”&gt;&lt;LI&gt;Teste&lt;/LI&gt;&lt;/UL&gt;

:arrow_right: Ordenada: Utiliza-se a TAG &lt;O&gt;&lt;&lt;/OL&gt; e &lt;LI&gt;&lt;/LI&gt;.
o Neste caso usa-se o comando “1”(ordenação numérica) ou “A”
(ordenação alfabética).

 Sintaxe: &lt;OL TYPE=”1”&gt;&lt;LI&gt;Teste&lt;/LI&gt;&lt;/OL&gt;

**TAGS DE FORMATAÇÃO**
&lt;b&gt;&lt;/b&gt; - negrito
&lt;i&gt;&lt;/i&gt; - itálico
&lt;u&gt;&lt;/u&gt; - sublinhado

**IMAGENS NO HTML**

:arrow_right: Pode-se inserir imagens de extenção JPEG, GIF ou PNG. Para isso
basta iniciar a TAG img.
Sintaxe: &lt; img src=”pasta/NomeDaImagem.extenção” /&gt;

**DIMENSÕES DA IMAGEM**

:arrow_right: Pode-se ajustar o tamanho de uma imagem, usando os parâmetros
width (largura) e height (altura), que podem ser dadas como pixels(px)
ou porcentagem(%).
 Sintaxe: &lt; img src=”IMAGENS/foto.png” width=”100px”
height=”100px” /&gt;
LINKS

:arrow_right: Permite a conexão entre documentos.

:arrow_right: Utiliza-se a TAG &lt; a &gt;. Dentro dela deverá ser informado o local e o
elemento, onde será exibido o link. Isso será possível através do
parâmetro “href”.
Sintaxe: &lt; a href=”destino”&gt; Este é o link &lt;/a&gt;.

**CSS**

:arrow_right: Cascading Style Sheets, significa em português, Folhas de Estilo em
Cascata.

:arrow_right: Facilita na fortamação do arquivo html, podendo fazer alterações de
forma prática. Nele voce pode fazer configuraçoes das imagens, de
tabelas, entre outros.

:arrow_right: Folhas de estilo INLINE:
o Sintaxe: &lt; tag style=”color: #000000; “&gt;
o No caso acima, iniciamos o atributo style e a cor dada, foi a preta.
Assim, o texto será exibido na cor preta.
o É possível escolher cores diversas, através da paleta de cores
html. No Google estao disponíveis vários modelos, basta escolher
a cor desejada e copiar o código dela.
o Tamanhos mais usados no font-size: small, medium, large, larger
e smaller.

 **Folhas de estilo externa:**

o É um arquivo com extensão CSS, que é atribuida ao arquivo html
com todas as formatações feitas.
o Deve ser armazenada na TAG &lt;head&gt;&lt;/head&gt;.
o Sintaxe: &lt; link rel=”stylesheet” type=”text/css”
href=”arquivo.css”/&gt;



Autora: Camila Lima
