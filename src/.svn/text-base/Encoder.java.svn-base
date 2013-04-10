import java.util.ArrayList;


public class Encoder {
	private String userphrase;
	private static final char[] Letters = {'a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z'};
	private static final String[] MorseLet = {".-","-...","-.-.","-..",".","..-.","--.","....","..",".---","-.-",".-..","--","-.","---",
		".--.","--.-",".-.","...","-","..-","...-",".--","-..-","-.--","--.."};
	

	private String InputPhrase;
	private String[] encodephrase;
	private int wordlength;

	public Encoder(String p) {
		InputPhrase = p;
		userphrase = p.toLowerCase();
		wordlength = userphrase.length();
		encodephrase = new String[wordlength];
		ChangeCode();

	}

	public void ChangeCode() {
		char[] letarray = userphrase.toCharArray();
		for(int i=0; i<wordlength; i++){
			for(int j=0; j<Letters.length; j++){
				if (letarray[i] == Letters[j]){
					encodephrase[i] = MorseLet[j];
				}
				if(letarray[i] == ' '){
					encodephrase[i]= "@";
				}

			}
		}
	}//end changecode

	public void OutputMorse(){
		System.out.println("\n" + "\"" + InputPhrase + "\"" + " In Morse Code is:\n\n");
		for(String s : encodephrase){
			if(s == "@"){
				System.out.print("   ");
			}
			else{
				System.out.printf("%s ",s);
			}
		}//end for



	}//end OutputMorse
}






