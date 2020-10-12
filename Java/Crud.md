####                            JAVA WEB COM BANCO DE DADOS

:arrow_right: **Por que usar um banco de dados?**

Os bancos de dados são usados para guardar informações. Através desse banco podemos fazer consultas de forma rápida e modificações caso preciso. Outra funcionalidade é a segurança de toda a informação por meio da devida proteção para evitar o roubo ou a danificação dos dados.

:arrow_right: **CRUD**

O significado dessa sigla é um acrônimo para as quatro operações básicas de banco de
dados,
C-create
R-read
U-update
D-delete

:arrow_right: **DAO (Objeto de acesso de dados)**

 É um padrão de processo para acesso de dados. Na prática a classe DAO são os CRUD. Dentro do DAO podem ser usadas somente as operações básicas do CRUD.

É por meio do CRUD que se torna possível linkar um banco de dados a um programa escrito em Java. Para isso, você deve baixar o servidor MYSQL, o Workbench e o mysql-connector instalados em seu computador. Baixe- os em:

MYSQL e Workbench: https://dev.mysql.com/downloads/installer/

mysql-connector: https://jar-download.com/download-handling.php

Instalados esses programas, vamos botar a mão na massa. Para tal, crie todos os pacotes e os arquivos dessa imagem:

​                                      ![lari1](https://github.com/Pedrogvd/Projeto_StartLatam/blob/main/Imagens_JAVA/lari1.jpg)

**Após isso, faça esse código no DAO:**



package br.com.GSCursos.dao;

import java.sql.Connection;
import java.sql.Date;
import java.sql.PreparedStatement;


import br.com.GSCursos.factory.ConnectionFactory;
import br.com.GSCursos.model.Alunos;
import br.com.GSCursos.model.Professores;

public class GSCursosDAO {

	public void save(Alunos alunos) {
		String sql= "INSERT INTO contatos(nome, nascimento, sexo, matricula, situacao) VALUES (?, ?, ?, ?, ?)";
		Connection conn= null;
		PreparedStatement pstm= null;
		try {
			
			conn= ConnectionFactory.createConnectionToMySQL();
			pstm= conn.prepareStatement(sql);
			pstm.setString(1, alunos.getNome());
			pstm.setDate(2, new Date(alunos.getNascimento().getTime()));
			pstm.setString(3, alunos.getSexo());
			pstm.setInt(4, alunos.getMatricula());
			pstm.setString(5, alunos.getSituacao());
			
			pstm.execute();


​			
		} catch (Exception e) {
			e.printStackTrace();
		}
		finally{
			try{
				if(pstm!=null) {
					pstm.close();
				}
				if(conn!=null) {
					conn.close();
				}
			}catch(Exception e){
				e.printStackTrace();
			}
		}


​	
	}public void save2 (Professores professores) {
		
		String sql= "INSERT INTO contatos(nome_prof, ch, salario, vha, qtdMaisDe65anos) VALUES (?, ?, ?)";
		Connection conn= null;
		PreparedStatement pstm= null;
		try {
			
			conn= ConnectionFactory.createConnectionToMySQL();
			pstm= conn.prepareStatement(sql);
			pstm.setString(1, professores.getNome_prof());
			pstm.setInt(2, professores.getCh());
			pstm.setDouble(3, professores.getSalario());
			pstm.setDouble(4, professores.getVha());
			pstm.setInt(5, professores.getQtdMaisDe65anos());
			pstm.execute();


​			
		} catch (Exception e) {
			e.printStackTrace();
		}
		finally{
			try{
				if(pstm!=null) {
					pstm.close();
				}
				if(conn!=null) {
					conn.close();
				}
			}catch(Exception e){
				e.printStackTrace();
			}
		}


​		
	}

}





**Depois, vá para o FACTORY e digite:**

package br.com.GSCursos.factory;
import java.sql.Connection;
import java.sql.DriverManager;
public class ConnectionFactory {
	
  private static final String USERNAME="root";
	
  private static final String PASSWORD=""; //aqui é a sua senha do Banco de Dados
  private static String DATABASE_URL="jdbc:mysql://localhost:3306/agenda?useTimezone=true&serverTimezone=UTC";

  public static Connection createConnectionToMySQL() throws Exception{
	  Class.forName("com.mysql.cj.jdbc.Driver");
	  Connection connection= DriverManager.getConnection(DATABASE_URL,USERNAME,PASSWORD);
	  return connection;
}

  public static void main(String[] args) throws Exception{
	  Connection con= createConnectionToMySQL();
	  if(con!=null) {
		  System.out.println("Conexão obtida com sucesso");
		  con.close();
	  }

  }
}



**Em seguida, digite na classe Alunos:**

package br.com.GSCursos.model;

import java.util.Date;

public class Alunos {
	private String nome;
	private Date nascimento;
	private String sexo;
	private int matricula;
	private String situacao;
	public String getNome() {
		return nome;
	}
	public void setNome(String nome) {
		this.nome = nome;
	}
	public Date getNascimento() {
		return nascimento;
	}
	public void setNascimento(Date nascimento) {
		this.nascimento = nascimento;
	}
	public String getSexo() {
		return sexo;
	}
	public void setSexo(String sexo) {
		this.sexo = sexo;
	}
	public int getMatricula() {
		return matricula;
	}
	public void setMatricula(int matricula) {
		this.matricula = matricula;
	}
	public String getSituacao() {
		return situacao;
	}
	public void setSituacao(String situacao) {
		this.situacao = situacao;
	}
}



**Após isso, digite na classe Professores:**

package br.com.GSCursos.model;

public class Professores {
	private String nome_prof;
	private int ch;
	private double salario;
	private double vha;
	private int qtdMaisDe65anos;
	public String getNome_prof() {
		return nome_prof;
	}
	public void setNome_prof(String nome_prof) {
		this.nome_prof = nome_prof;
	}
	public int getCh() {
		return ch;
	}
	public void setCh(int ch) {
		this.ch = ch;
	}
	public double getSalario() {
		return salario;
	}
	public void setSalario(double salario) {
		this.salario = salario;
	}
	public double getVha() {
		return vha;
	}
	public void setVha(double vha) {
		this.vha = vha;
	}


	public int getQtdMaisDe65anos() {
		return qtdMaisDe65anos;
	}
	public void setQtdMaisDe65anos(int qtdMaisDe65anos) {
		this.qtdMaisDe65anos = qtdMaisDe65anos;
	}
	
	}
	
Por fim, vá para a classe Main e teste valores:

package br.com.GSCursos.aplicacao;

import java.util.Date;

import br.com.GSCursos.dao.GSCursosDAO;
import br.com.GSCursos.model.Alunos;
import br.com.GSCursos.model.Professores;

public class Main {
public static void main (String[] args) {
	//fiz alguns exemplos só pra aparecer no banco de dados
	Professores professores = new Professores ();
	Alunos alunos = new Alunos ();
	GSCursosDAO gscursosdao = new GSCursosDAO();
	alunos.setNome("Pedro Gabriel");
	alunos.setMatricula(6865);
	alunos.setNascimento(new Date());
	alunos.setSexo("masculino");
	alunos.setSituacao("aprovação");
	gscursosdao.save(alunos);
	
	professores.setCh(24);
	professores.setQtdMaisDe65anos(1);
	professores.setSalario(3000);
	professores.setVha(35);
	professores.setNome_prof("Ana Paula");
	gscursosdao.save2(professores);
}
}



*Créditos ao código: Pedro Gabriel Vilaça Diniz --> instagram: @Pedrogvd*





Autora: Larissa Caroline
