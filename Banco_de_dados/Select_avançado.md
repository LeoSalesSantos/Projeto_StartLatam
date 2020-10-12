####                                         **SQL - Manipulação de dados**

#####                                                               Select avançado

Filtros:

 **WHERE** **-** O comando where possibilita que os resultados das consultas sejam filtrados. 
![tabela 1](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_BD/tabela.PNG)

SELECT * FROM SALA WHERE NOTA = 7; 

SELECT * FROM SALA WHERE NOTA < > 10;

SELECT * FROM SALA WHERE NOTA >= 7; 

SELECT * FROM SALA WHERE NOTA <= 7; 

SELECT * FROM SALA WHERE NOTA < 7;

SELECT * FROM SALA WHERE NOTA > 7;




 **BETWEEN** **-** Recebe um valor mínimo e um valor máximo e retorna os dados da coluna que atendem a esse critério.

SELECT * FROM SALA WHERE nota BETWEEN 3 AND 7;



**LIKE** **-**  Permite comparar o valor de uma coluna com uma sequências de caracteres. Esse operador permite o uso do sinal de porcentagem (%),
 que substitui um ou mais caracteres.
        SELECT * FROM SALA WHERE alunoLIKE ‘%Silva%’;

SELECT * FROM SALA WHERE alunoNOT LIKE ‘%Silva%’;



 **IN** **-** Com este operador podemos criar uma lista de valores que serão comparados com o valor na coluna. 
SELECT * FROM SALA WHERE ID IN (1,3); 



 **AND -** Utilizado para unir duas ou mais condições, o operador "and" serve como "E"(visto em operações lógicas).
SELECT * FROM SALA WHERE NOTA < > 10 AND MATERIA LIKE ‘%Geografia%’;



 **OR -** Assim como o "AND", o "OR" também é utilizados para unir condições, mas a sua função é parecida com o "OU" (visto em operações lógicas).
 SELECT * FROM SALA WHERE LIKE ‘%Matemática%’ OR MATERIA LIKE ‘%Geografia%’;



**ORDER BAY -** Usado para ordenar o resultado da consulta em banco de dados, com ele pode-se ordenar utilizando qualquer coluna da tabela.
 SELECT NOME SALA WHERE NOTA > 1 ORDER BY NOME; 
 SELECT NOME FROM SALA ORDER BY NOTA; 
 Se precisar que as informações virem em ordem decrescente acrescenta-se após o nome do campo a palavra DESC.
 SELECT NOME SALA WHERE NOTA > 1 ORDER BY NOME DESC; 
 SELECT NOME FROM SALA ORDER BY NOTA DESC;



Autora: Rayane Souza
