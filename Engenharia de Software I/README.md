## Gabriele Stephanie Silva de Oliveira RA: 1460742111012	

## Diagrama de caso de uso

### Requisitos Funcionais

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/img/caso-de-uso.png">

## Requisitos Não Funcionais

<img src = "https://github.com/oliveira-gabriele/bertoti/blob/main/Engenharia%20de%20Software%20I/img/%2310%20Heuristics.png">

## #1: Visibilidade do status do sistema
Apresenta um feedback claro do estado do usuário, facilitando assim a identificação. Verde - online, Amarelo - ausente e Vermelho - ocupado.

## #2: Jogo entre sistema e o mundo real
Ícones que condizem com a realidade, tornando a navegação pela interface intuitiva e rápida, poupando o usuário de perder seu tempo.

## #3: Controle e liberdade do usuário
Botão voltar que facilita a navegação entre os menus.

## #4: Consistência e padrões
A tela principal sempre será os blocos das disciplinas.

## #5: Prevenção de erros
Para prevenir erros ao adicionar um arquivo errado na aba de tarefas existe uma opção de remover o arquivo, caso o mesmo já tenha sido enviado um botão desfazer sempre aparecerá após cada entrega.

## #6: Reconhecimento em vez de recordação
Com o foco em diminuir as informações que os usuários têm que lembrar, um menu com atalhos para Calendário, Chat, Disciplinas, Tarefas e Configurações é encontrado na parte inferior.

## #7: Flexibilidade e eficiência de uso
Para acelerar a trocar entre os menus, a interface possui atalhos como: T - Tarefas, C - Chat e D - Disciplinas.

## #8: Design estético e minimalista
As informações apresentadas na tela são simples e objetivas, de forma que o usuário não perda o foco e se distraia, mantendo assim a produtividade.

## #9: Ajude os usuários a reconhecer, diagnosticar e recuperar de erros
Uma placa simbolizando a falta de acesso à internet será exibida no centro da tela caso a conexão do usuário caia, auxiliando a identifição do erro por ele.

## #10: Ajuda e documentação
A fim de suprir incertezas do cliente no inferior direito da interface há um ícone que leva até o manual de instruções, contendo o passo a passo de cada funcionalidade do sistema. 

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




