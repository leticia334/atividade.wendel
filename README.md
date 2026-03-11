2#TABUADAOPERACOES
import java.util.Scanner;

public class TabuadaOperacoes {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Digite um número: ");
        int num = sc.nextInt();

        System.out.println("\nTabuada de Adição:");
        for(int i = 1; i <= 10; i++){
            System.out.println(num + " + " + i + " = " + (num + i));
        }

        System.out.println("\nTabuada de Subtração:");
        for(int i = 1; i <= 10; i++){
            System.out.println(num + " - " + i + " = " + (num - i));
        }

        System.out.println("\nTabuada de Multiplicação:");
        for(int i = 1; i <= 10; i++){
            System.out.println(num + " x " + i + " = " + (num * i));
        }

        System.out.println("\nTabuada de Divisão:");
        for(int i = 1; i <= 10; i++){
            System.out.println(num + " / " + i + " = " + (num / (double)i));
        }

        sc.close();
    }
}




#MULTIPLOS
import java.util.Scanner;

public class multiplo{

    public static void main(String[]args){
        Scanner sc = new Scanner(System.in);
        System.out.print(" digite o primeiro numero: ");
        int n1 = sc.nextInt();

        System.out.print("digite o segundo numero: ");
        int n2 = sc.nextInt();

        int inicio = Math.min(n1, n2);
        int fim = Math.max(n1, n2);
        
        System.out.println("Múltiplos de 3 em ordem crescente: ");
        for (int i =inicio; i <=fim; i++){
            if (i % 3 == 0){
                System.out.println(i);

         }

        }
        System.out.println("Múltiplos de 3 em ordem de765crescente: ");
        for (int i = fim; i>= inicio; i--){
            if(i % 3 == 0) {
                System.out.println(i);
            }
        }
         
        sc.close();
        }
    }
    
    



#MULTIPLOS3 
import java.util.Scanner;

public class MultiplosDe3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Digite o primeiro número: ");
        int n1 = sc.nextInt();

        System.out.print("Digite o segundo número: ");
        int n2 = sc.nextInt();

        if (n1 < n2) {
            // ordem crescente
            for (int i = n1; i <= n2; i++) {
                if (i % 3 == 0) {
                    System.out.println(i);
                }
            }
        } else {
            // ordem decrescente
            for (int i = n1; i >= n2; i--) {
                if (i % 3 == 0) {
                    System.out.println(i);
                }
            }
        }

        sc.close();
    }
}




#SENHA
import java.util.Scanner;

public class Senha {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int senhaCorreta = 1234;
        int senha;

        System.out.print("Digite a senha: ");
        senha = sc.nextInt();

        while (senha != senhaCorreta) {
            System.out.println("Senha incorreta! Tente novamente.");
            System.out.print("Digite a senha: ");
            senha = sc.nextInt();
        }

        System.out.println("Senha correta! Acesso permitido.");

        sc.close();
    }
}




#PRIMOS
public class Primos {
    public static void main(String[] args) {

        int soma = 0;

        for (int i = 2; i <= 50; i++) {
            boolean primo = true;

            for (int j = 2; j < i; j++) {
                if (i % j == 0) {
                    primo = false;
                    break;
                }
            }

            if (primo) {
                System.out.println(i);
                soma += i;
            }
        }

        System.out.println("Soma dos números primos: " + soma);
    }
}




POTENCIASEMFUÇAO
import java.util.Scanner;

public class PontenciaSemFunçao {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        int base, expoente;
        int resultado = 1;

        System.out.print("Digite o primeiro número (base): ");
        base = sc.nextInt();

        System.out.print("Digite o segundo número (expoente): ");
        expoente = sc.nextInt();

        for (int i = 1; i <= expoente; i++) {
            resultado = resultado * base;
        }

        System.out.println("Resultado: " + resultado);

        sc.close();
    }
}




   
