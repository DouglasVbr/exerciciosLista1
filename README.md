# exerciciosLista1


package lista1;


 
  // @author Douglas
public class Lista1 {

    
    public static void main(String[] args) {
        
         // Criando uma instância da classe Exercicio1
        Exercicio1 exercicio1 = new Exercicio1();
        // Chamando o método para imprimir "Olá, mundo!"
        exercicio1.imprimirMensagem();
        
        // Criando uma instância da classe Exercicio2
        Exercicio2 exercicio2 = new Exercicio2();
        // Chamando o método para capturar o nome e exibir a mensagem
        exercicio2.saudacao();
        
         // Criando uma instância da classe Exercicio3
        Exercicio3 exercicio3 = new Exercicio3();
        // Chamando o método para concatenar e imprimir a mensagem
        exercicio3.concatenarStrings();
        
          // Criando uma instância da classe Exercicio4
        Exercicio4 exercicio4 = new Exercicio4();
        // Chamando o método para realizar as operações de String
        exercicio4.manipularString();
        
        
        
    }

    
    
    
}


package lista1;

/**
 *
 * @author Douglas
 */
public class Exercicio1 {
    // Método que imprime "Olá, mundo!" no console
    public void imprimirMensagem() {
        System.out.println("Olá, mundo!");
    }
}



package lista1;
/**
 *
 * @author Douglas
 */
import java.util.Scanner;

public class Exercicio2 {
    // Método que captura o nome do usuário e imprime a mensagem de boas-vindas
    public void saudacao() {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite seu nome: ");
        String nome = scanner.nextLine();
        System.out.println("Olá, " + nome + "! Bem-vindo ao programa.");
    }
}



package lista1;

/**
 *
 * @author Douglas
 */
public class Exercicio3 {
    
    
    // Método que concatena duas strings e imprime a mensagem completa
    public void concatenarStrings() {
        String parte1 = "Olá,";
        String parte2 = " mundo!";
        String mensagemCompleta = parte1 + parte2;
        System.out.println(mensagemCompleta);
        }
}


package lista1;

/**
 *
 * @author Douglas
 */
public class Exercicio4 {
    
    // Método que realiza as operações de String e imprime os resultados
    public void manipularString() {
        String frase = "Esta é uma frase de exemplo para exercício.";

        // 1. Determine e imprima o tamanho da frase.
        int tamanho = frase.length();
        System.out.println("Tamanho da frase: " + tamanho);

        // 2. Converta a frase para letras maiúsculas e imprima o resultado.
        String maiuscula = frase.toUpperCase();
        System.out.println("Frase em maiúsculas: " + maiuscula);

        // 3. Converta a frase para letras minúsculas e imprima o resultado.
        String minuscula = frase.toLowerCase();
        System.out.println("Frase em minúsculas: " + minuscula);

        // 4. Extraia a substring "frase de exemplo" da frase original e imprima-a.
        String subString = frase.substring(11, 26);
        System.out.println("Substring extraída: " + subString);
    }
    
}

# exerciciosLista2


package lista2;

import java.util.Scanner; 

/**
 *
 * @author Douglas
 */
public class Lista2 {

    
    public static void main(String[] args) {
        
        Scanner scanner = new Scanner(System.in);

        // Exercício 1: Contagem de Letras
        System.out.print("Exercício 1 - Digite uma palavra: ");
        String palavra = scanner.nextLine();
        ContagemDeLetras.exercicio(palavra);

        // Exercício 2: Substituição de Caracteres
        System.out.print("Exercício 2 - Digite uma frase: ");
        String frase = scanner.nextLine();
        SubstituicaoDeCaracteres.exercicio(frase);

        // Exercício 3: Inversão de Palavra
        System.out.print("Exercício 3 - Digite uma palavra: ");
        palavra = scanner.nextLine();
        InversaoDePalavra.exercicio(palavra);

        // Exercício 4: Verificação de Palíndromo
        System.out.print("Exercício 4 - Digite uma palavra: ");
        palavra = scanner.nextLine();
        VerificacaoDePalindromo.exercicio(palavra);

        // Exercício 5: Contagem de Palavras
        System.out.print("Exercício 5 - Digite uma frase: ");
        frase = scanner.nextLine();
        ContagemDePalavras.exercicio(frase);

        // Exercício 6: Capitalização de Nomes
        System.out.print("Exercício 6 - Digite seu nome completo: ");
        String nomeCompleto = scanner.nextLine();
        CapitalizacaoDeNomes.exercicio(nomeCompleto);

        // Exercício 7: Extração de Domínio de Email
        System.out.print("Exercício 7 - Digite seu email: ");
        String email = scanner.nextLine();
        ExtracaoDeDominioEmail.exercicio(email);

        // Exercício 8: Mascaramento de Informações
        System.out.print("Exercício 8 - Digite o número do seu cartão de crédito: ");
        String numeroCartao = scanner.nextLine();
        MascaramentoDeInformacoes.exercicio(numeroCartao);

        // Exercício 9: Remoção de Espaços Extras
        System.out.print("Exercício 9 - Digite uma frase com espaços extras: ");
        frase = scanner.nextLine();
        RemocaoDeEspacosExtras.exercicio(frase);

        // Exercício 10: Contagem de Vogais e Consoantes
        System.out.print("Exercício 10 - Digite uma palavra: ");
        palavra = scanner.nextLine();
        ContagemDeVogaisEConsoantes.exercicio(palavra);

        scanner.close();
 
        
    }
    
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class CapitalizacaoDeNomes {
    
      public static void exercicio(String nomeCompleto) {
        String[] palavras = nomeCompleto.split("\\s+");
        StringBuilder nomeFormatado = new StringBuilder();
        for (String palavra : palavras) {
            nomeFormatado.append(Character.toUpperCase(palavra.charAt(0)))
                         .append(palavra.substring(1).toLowerCase())
                         .append(" ");
        }
        System.out.println("Nome formatado: " + nomeFormatado.toString().trim());
    }
    
}



package lista2;

/**
 *
 * @author Douglas
 */
public class ContagemDeLetras {
    
     public static void exercicio(String palavra) {
        System.out.println("A palavra '" + palavra + "' tem " + palavra.length() + " letras.");
    }
    
}

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class ContagemDePalavras {
    
     public static void exercicio(String frase) {
        String[] palavras = frase.trim().split("\\s+");
        System.out.println("A frase contém " + palavras.length + " palavras.");
    }
    
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class ContagemDeVogaisEConsoantes {
    
    public static void exercicio(String palavra) {
        int vogais = 0;
        int consoantes = 0;
        String palavraLower = palavra.toLowerCase();
        for (char c : palavraLower.toCharArray()) {
            if (c >= 'a' && c <= 'z') {
                if ("aeiou".indexOf(c) != -1) {
                    vogais++;
                } else {
                    consoantes++;
                }
            }
        }
        System.out.println("A palavra '" + palavra + "' tem " + vogais + " vogais e " + consoantes + " consoantes.");
    }
    
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class ExtracaoDeDominioEmail {
    
     public static void exercicio(String email) {
        int posicaoArroba = email.indexOf('@');
        if (posicaoArroba != -1) {
            String dominio = email.substring(posicaoArroba + 1);
            System.out.println("Domínio: " + dominio);
        } else {
            System.out.println("Email inválido.");
        }
    }
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class InversaoDePalavra {
    
     public static void exercicio(String palavra) {
        String palavraInvertida = new StringBuilder(palavra).reverse().toString();
        System.out.println("Palavra invertida: " + palavraInvertida);
    }
    
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class MascaramentoDeInformacoes {
    
     public static void exercicio(String numeroCartao) {
        String mascarado = "************" + numeroCartao.substring(numeroCartao.length() - 4);
        System.out.println("Número do cartão: " + mascarado);
    }
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class RemocaoDeEspacosExtras {
    
     public static void exercicio(String frase) {
        String fraseFormatada = frase.trim().replaceAll("\\s+", " ");
        System.out.println("Frase formatada: " + fraseFormatada);
    }
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class SubstituicaoDeCaracteres {
    
    public static void exercicio(String frase) {
        String fraseModificada = frase.replace('a', '*').replace('A', '*');
        System.out.println("Frase modificada: " + fraseModificada);
    }
    
}


/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Classes/Class.java to edit this template
 */
package lista2;

/**
 *
 * @author Douglas
 */
public class VerificacaoDePalindromo {
    
     public static void exercicio(String palavra) {
        String palavraInvertida = new StringBuilder(palavra).reverse().toString();
        if (palavra.equalsIgnoreCase(palavraInvertida)) {
            System.out.println("A palavra '" + palavra + "' é um palíndromo.");
        } else {
            System.out.println("A palavra '" + palavra + "' não é um palíndromo.");
        }
    }
    
}












