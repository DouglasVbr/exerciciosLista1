# exerciciosLista1
** pagina main

package pooii;

import java.util.Scanner;

/**
 *
 * @author Douglas Vieira
 */

//lista 1
public class PooII extends exer2 {

    
   
    public static void main(String[] args) {
        // exercicio1
        System.out.println("olá, mundo");
        
        //exercicio2
        Scanner scanner = new Scanner (System.in);
        exer2 saudacao = new exer2();
        
        String nome = saudacao.capturarNome(scanner);
        
        System.out.println(" olá " + nome + "! bem-vindo ao programa. ");
        
        
        scanner.close();
        
        //exercicio3
        
        exer3 concatenacao = new exer3();
        
        String ola = "olá,";
        String complemento = "mundo!";
        
        String mensagemCompleta = concatenacao.concatenarString(ola, complemento);
        
        
        System.out.println(mensagemCompleta);
    }

   
    
    
}

package pooii;


public class exer01 {
    String msg = "olá, mundo";

    public String getMsg() {
        return msg;
    }
    
    
}

package pooii;


import java.util.Scanner;

public class exer2 {

    public String capturarNome(Scanner scanner) {
        System.out.println("Digite seu Nome: ");
        

        return scanner.nextLine();

    }

}



package pooii;


public class exer3 {
    
    public String concatenarString(String str1, String str2){
    
        return str1 + str2;
    }
    
}








