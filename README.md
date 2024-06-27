# desafio-dio-dontrole
# desafio-dio-dontrole



package desafio;

import java.util.Scanner;

public class Contador {

	public static void main(String[] args) {
		Scanner terminal = new Scanner(System.in);
		System.out.println("Digite o primeiro parâmetro");
		int parametroUm = terminal.nextInt();
		System.out.println("Digite o segundo parâmetro");
		int parametroDois = terminal.nextInt();
		
		try {
			
			contar(parametroUm, parametroDois);
		
		}catch (ParametrosInvalidosException erro) {
			
			
			System.out.println("Segundo parâmetro deve ser maior que o Primeiro" +erro.getMessage());
		}
		
	}
	
	
	static void contar(int parametroUm, int parametroDois ) throws ParametrosInvalidosException {
		if(parametroUm > parametroDois) {
		
		}
		
		int contagem = parametroDois - parametroUm;
		int primeiro = 0;
		for(int i = primeiro; i <= contagem; i++) {
			System.out.println("Imprimir número: " +i);
		} 
		
		
	}
	
	 class ParametrosInvalidosException extends Exception{
	        public ParametrosInvalidosException (String message) {
	            super(message);
	        }
	    }

}
