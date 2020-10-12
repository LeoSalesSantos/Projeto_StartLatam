####                                                    **SQL**

*Chave Primária:* é uma parte da tabela onde se encontra um registro
específico, ele é identificado por ter um valor único, nenhum valor se repete

*Chave Estrangeira:* é a chave em outra tabela para descobrir o valor da sua
tabela de origem quando necessário.

**Tipos de Dados**
Unsigned (Sem sinal)

**AUTO_INCREMENT**
Preenche automaticamente um campo da tabela do tipo int quando adicionamos
elementos em uma determinada linha.
Exemplo: ID int AUTO_INCREMENT
ZEROFILL
Preenche espaços vazios da coluna com o número zero.
Exemplo: Uma coluna que é declarada como
INT(4) ZEROFILL, o valor 5 é recuperado como
0005.

:arrow_right: Unique: Impede que haja valores repetidos da chave primária da mesma tabela.
Exemplo: Id int NOT NULL UNIQUE
Obs: Uma restrição PRIMARY KEY tem automaticamente uma restrição UNIQUE

#### Inserindo dados nas tabelas (INSERT)

Inicie sempre inserindo os dados das tabelas sem chaves
estrangeiras.
CREATE TABLE empresa.setor (
Id_setor integer PRIMARY KEY,
Nome_setor Varchar(50) not null);INSERT INTO empresa.setor ( Id_setor, Nome_setor
) VALUES
(99,&#39;ADMINISTRAÇÃO&#39;);
Para visualizar todos os dados que foram inseridos devemos
utilizar o seguinte comando:
SELECT* FROM empresa.setor;
1

O **UPDATE** é utilizado para a atualização de um registro já existente, por exemplo
temos um registro onde um funcionário mudou de cargo, e para alterarmos no banco
utilizamos como condição o nome da pessoa.
UPDATE empresa.funcionario
SET cargo = 33
WHERE NOME = &#39;BARBARA&#39;;

O **DELETE** funciona para retirarmos um registro da tabela. Como no UPDATE deve-se
utilizar o WHERE para que seja filtrado quais registros devem ser deletados. Como
exemplo, iremos deletar a funcionária Ana, por ela ter saído da empresa:
:arrow_right: DELETE FROM empresa.funcionario WHERE id_funcionario = 11;



Autora: Kethelen Vieira

