# verificaanobissexto


package verificaanobissexto;
import java.util.Scanner;
public class VerificaAnoBissexto {

    
    public static void main(String[] args) {
        
     Scanner Scanner = new Scanner(System.in);
     // solicita ao usuario que insira o ano
     
        System.out.println("Digite o ano:");
        int ano = Scanner.nextInt();
        // verifica se o ano é bissexto
        boolean ehbissexto=false;
        if((ano % 4 == 0 && ano % 100 != 0)||( ano % 400 == 0)){
     ehbissexto=true; 
     }
        //exibe o resultado 
        if(ehbissexto){
            System.out.println(ano + " é um ano bissexto.");
        }else{
            System.out.println( ano + " não é um ano bissexto.");
        }
        // fecha o Scanner
        Scanner.close();
    
}
}
