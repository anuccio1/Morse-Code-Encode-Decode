import java.util.InputMismatchException;
import java.util.Scanner;


public class MorseCodeTester {


	public static void main(String[] args) {

		int choice=0;
		String phrase,code;
		boolean cont = true;

		Scanner input = new Scanner(System.in);

		do{

			try{
				System.out.println("Would You Like to Encode an English Phrase into Morse Code, or decode Morse code into an english phrase?");
				System.out.println("\n1.Encode");
				System.out.println("2.Decode");

				choice = input.nextInt();
				if(choice < 1 || choice > 2){
					while(choice < 1 || choice > 2){
						System.out.println("Invalid Input.");
						System.out.println("\n1.Encode");
						System.out.println("2.Decode");
						choice = input.nextInt();
					}
				}
				cont=false;
			}
			catch(InputMismatchException in){
				System.out.println("Invalid Input");
				input.nextLine();
			}

		} while(cont);				

		if(choice == 1){
			phrase = "whats up man";
			Encoder encode = new Encoder(phrase);
			encode.OutputMorse();

		}

		if(choice == 2){
			code = ".-- .... .- - ...    ..- .--.    -- .- -.";
			Decoder decode = new Decoder(code);
			

		}

	}



}
