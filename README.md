# Indicador-de-Passagem
import java.util.Scanner;

public class IndicadorDePassagem {

	public static void main(String[] args) {
		Scanner in = new Scanner(System.in);

		System.out.println("Digite numeros nao negativos (zero termina): ");

		int num = in.nextInt();
		boolean acheiUmImpar = false;
		
		while(num>0){
			if(num%2!=0){
				System.out.println("uuiii entrei");
				acheiUmImpar = true;
			}
			num = in.nextInt();
		}

		if(acheiUmImpar){
			System.out.println("Foi encontrado pelo menos um numero impar.");
		}else{
			System.out.println("Apenas numeros pares foram digitados.");
		}
		
		
		in.close();
	}

}
