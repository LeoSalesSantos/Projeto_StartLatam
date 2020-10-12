####                               **FRONT-END: Trabalha na parte visual (exterior)** 

Exemplo: Logo da página (login);

Estudo das cores: Matriz, Tom e Intensidade ;

Quando queremos mudar a cor do nosso projeto, basta somente usar o nome da cor em Inglês. Exemplo: “Black” ou pelo código da cor exemplo: “#RRGGBB

Herança: Trabalha as ligações do HTML, podemos usar como exemplo uma árvore genealógica de uma família, estão todos ligados e estão relacionados.

Entendendo melhor, podemos usar as tabelas: Facilita na organização de forma tabular em uma página web, contendo ( Textos, Links, Figuras, Etc);

**Estrutura de uma tabela**

< table > < /table > Define que é uma tabela

< th > < /th > Define o cabeçalho

< tr > < /tr > define as linhas

< td > < /td > define as colunas

Tabelas – Border: Definindo a espessura da borda

“Espessura_da_borda”

Table,th,td {

Border= 1 px solid black;

 {

Exemplo HTML: < table border="1" > ...< /table >

Exemplo Css: Style=”border: 1px solid black:” 

Largura da tabela: utilizamos a propriedade “width”

Em Pixels ou porcentagem

Sintaxe: < table width="150%> ...< /table > 

               <table width=”200px> ...</table>

Altura da Tabela: Usamos a propriedade “height” no HTML

Em Pixels ou e porcentagem

Sintaxe: < table height="200%" > ...< /table >

              <table height=”600px”> ...</table>

No CSS Usamos os dois juntos

Exemplo: table{

​               Width:200px

​               Height:600px

​          {

Cor no fundo da Tabela: Usamos a propriedade “bgcolor”

Pode ser aplicada as tags da tabela “< table >, < tr >, < th > ou < td >

Exemplo: < tr bgcolor="black" >

No CSS basta inserir da seguinte forma: tr{background-color.black;} ou no < td >...

**Alinhamento nas células**

Usamos as propriedades “ align para alinhamento horizontal e valign para vertical”

São aplicadas nas tags: < td > e < tr >

No CSS usamos o “text-align e vertical align” 

Exemplo: tr{ text-align: center

​            Vertical-align:top 

​          {

**ID**

Pensando em ID, pensamos logo em um identificador.

Por via de regra, utilizamos o CSS para gerar conjunto de regras que serão utilizadas pelas diversas tags HTML, podendo ser utilizadas em diversas tags.

**CCS ID**

Devemos identificar a tag como id

Exemplo: < td id="alinhamento1" >

Depois de criado a estrutura identificamos o elemento através do #

Exemplo 

\#alinhamento1 { text-align:center;

​                          Vertical-

​                    Align:middle;}

**Mesclando linhas e colunas** 

Para mesclar coluna utilizamos o “colspan” dentro de < th > ou < td >

Exemplo: 

< th colspan="2" >gênero< /th >

Para mesclar linha utilizamos o “rowspan” dentro de < th > ou < td >

Exemplo:

 < th rowspan="2" >gênero< /th >

< th >feminiino< /th >

< td >20< /td >

**Herança**

Podemos analisar e vermos o grau de parentesco nos elementos HTML;

HTML é o ai de head e body

Table é o pai de tf e avô de 4 td

Title é o filho de head

Temos os irmãos tr e td

Title e table são descendentes de HTML 

Table, body e html são ancestrais de td

Herança no CSS

**Trocando a cor do texto no CSS usando comente o código:**

 p{

Color:green;

{



(Até o que está em negrito muda de cor)

Agora se quisermos que a parte que está em negrito não mude utilizamos o seguinte código;

p{ color:green}

P{ color:blue;}

**CSS HOVER**

O “hover” é muito utilizado em links e menus de navegação, imagens e outros.

Exemplo:

P:hover{

​       Color:red;

}

Pronto, agora quando passar o mouse sobre o parágrafo, ele mudará de cor.

Também podemos fazer uma imagem aumentar de tamanho passando o mouse em cima, usando as seguintes tags:

Img:hover{

​         Width:110%

​         Height:110%



Autora: Ianca Nicole