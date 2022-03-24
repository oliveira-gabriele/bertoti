## Gabriele Stephanie Silva de Oliveira RA: 1460742111012	

## Diagrama de caso de uso

### Requisitos Funcionais

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/caso-de-uso.png">

## Requisitos Não Funcionais



## Diagrama de classe UML

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/Diagrama%20de%20Classe.png">


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

public class Pessoa{
	
	private int ra;
	private String nome;
	private String tipo;
	
	public Pessoa(int ra, String nome, String tipo) {
		this.ra = ra;
		this.placa = placa;
		this.espec = espec;
	}


	public int getRa(){
		return ra;
	}
	
	public void setRa(String novaPlaca){
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
public class Disciplina{
	
	private String matéria;
		
	public Pessoa(String matéria) {
		this.placa = placa;
	}

	public String getMatéria(){
		return matéria;
	}
	
	public void setMatéria(String novaMatéria){
		matéria = novaMatéria;
	}





