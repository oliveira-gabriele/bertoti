## Gabriele Stephanie Silva de Oliveira RA: 1460742111012	

## Diagrama de caso de uso

### Requisitos Funcionais

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/img/caso-de-uso.png">

## Requisitos Não Funcionais

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/img/%2310%20Heuristics.png">

#1: Visibilidade do status do sistema

#2: Jogo entre sistema e o mundo real

#3: Controle e liberdade do usuário

#4: Consistência e padrões

#5: Prevenção de erros

#6: Reconhecimento em vez de recordação

#7: Flexibilidade e eficiência de uso

#8: Design estético e minimalista

#9: Ajude os usuários a reconhecer, diagnosticar e recuperar de erros

#10: Ajuda e documentação

## Diagrama de classe UML

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/img/UML.drawio.png">

## Desenvolvimento do Código 

### Classe Plataforma de Ensino

~~~java

import java.util.LinkedList;
import java.util.List;

public class Plataforma de Ensino{

     private List<Pessoa> pessoas = new LinkedList<Pessoa>();

     public void cadastrarPessoa(Pessoa pessoas){
          pessoas.add(pessoas);
     }

     public List<Pessoa> buscarPessoaNome(String nome){
           List<Pessoa> encontradas = new LinkedList<Pessoa>();
           for(Pessoa pessoa:pessoas){
                if(pessoa.getNome().equals(nome)) encontradas.add(pessoa);
           }
           return encontradas;
     }

     public Pessoa buscarRa(int Ra){
          for(Pessoa pessoa:pessoas){
               if(pessoa.getRa().equals(Ra)) return pessoa; 
          }
          return null;
     }

     public List<Pessoa> getPessoas(){
           return pessoas;
     }
}

~~~~

### Classe Pessoa

~~~java

public class Pessoa{
	
	private int ra;
	private String nome;
	private String tipo;
	
	public Pessoa(int ra, String nome, String tipo) {
		this.ra = ra;
		this.nome = nome;
		this.tipo = tipo;
	}


	public int getRa(){
		return ra;
	}
	
	public void setRa(String novoRa){
		ra = novoRa;
	}

	public String getNome(){
		return nome;
	}
	
	public void setNome(String novoNome){
		nome = novoNome;
	}

	public String getTipo(){
		return tipo;
	}
	
	public void setTipo(String novoTipo){
		tipo = novoTipo;
	}

}

~~~~

### Classe Disciplina

~~~java

public class Disciplina{
	
	private String matéria;
		
	public Matéria(String matéria) {
		this.matéria = matéria;
	}

	public String getMatéria(){
		return matéria;
	}
	
	public void setMatéria(String novaMatéria){
		matéria = novaMatéria;
	}
~~~




