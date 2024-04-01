# Express-es-matematica

package pesoaltura;

import java.util.Scanner;

public class Pesoaltura {

	public static void main(String[] args) {
		 Scanner scanner = new Scanner(System.in);
	        
	        System.out.print("Digite a altura em metros: ");
	        double altura = scanner.nextDouble();
	        
	        System.out.print("Digite o sexo (M para masculino ou F para feminino): ");
	        char sexo = scanner.next().charAt(0);
	        
	        double pesoIdeal;
	        
	        if (sexo == 'M' || sexo == 'm') {
	            pesoIdeal = (72.7 * altura) - 58;
	            System.out.println("O peso ideal para um homem com " + altura + " metros de altura é aproximadamente " + pesoIdeal + " kg.");
	        } else if (sexo == 'F' || sexo == 'f') {
	            pesoIdeal = (62.1 * altura) - 44.7;
	            System.out.println("O peso ideal para uma mulher com " + altura + " metros de altura é aproximadamente " + pesoIdeal + " kg.");
	        } else {
	            System.out.println("Sexo não reconhecido. Por favor, insira 'M' para masculino ou 'F' para feminino.");
	        }
	        
	        scanner.close();

	}

}
