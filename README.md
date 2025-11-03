# JAVA-Lista-Exercicios
40 Programas Java

# --------- 1 a 10 (uso de IF) ----------
criar_java "LESM01 'package luiseduardo;
import java.util.Scanner;
public class LESM01 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Digite um número inteiro: ");
        int n = sc.nextInt();
        if (n > 0) System.out.println("Número positivo");
        else if (n < 0) System.out.println("Número negativo");
        else System.out.println("Zero");
        sc.close();
    }
}'

criar_java "LESM02" 'package luiseduardo;
import java.util.Scanner;
public class LESM02 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Digite um número: ");
        int n = sc.nextInt();
        System.out.println((n % 2 == 0) ? "Par" : "Ímpar");
        sc.close();
    }
}'

criar_java "LESM03" 'package luiseduardo;
import java.util.Scanner;
public class LESM03 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Primeiro número: ");
        double a = sc.nextDouble();
        System.out.print("Segundo número: ");
        double b = sc.nextDouble();
        if (a > b) System.out.println("Maior: " + a);
        else if (b > a) System.out.println("Maior: " + b);
        else System.out.println("São iguais");
        sc.close();
    }
}'

criar_java "LESM04" 'package luiseduardo;
import java.util.Scanner;
public class LESM04 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Digite sua idade: ");
        int idade = sc.nextInt();
        System.out.println(idade >= 16 ? "Pode votar" : "Não pode votar");
        sc.close();
    }
}'

criar_java "LESM05" 'package luiseduardo;
import java.util.Scanner;
public class LESM05 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Nota 1: ");
        double n1 = sc.nextDouble();
        System.out.print("Nota 2: ");
        double n2 = sc.nextDouble();
        double media = (n1 + n2) / 2;
        System.out.println("Média: " + media);
        System.out.println(media >= 7 ? "Aprovado" : "Reprovado");
        sc.close();
    }
}'

criar_java "LESM06" 'package luiseduardo;
import java.util.Scanner;
public class LESM06 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Número: ");
        int n = sc.nextInt();
        if (n % 3 == 0 && n % 5 == 0) System.out.println("Múltiplo de 3 e 5");
        else if (n % 3 == 0) System.out.println("Múltiplo de 3");
        else if (n % 5 == 0) System.out.println("Múltiplo de 5");
        else System.out.println("Não é múltiplo de 3 nem 5");
        sc.close();
    }
}'

criar_java "LESM07" 'package luiseduardo;
import java.util.Scanner;
public class LESM07 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Lado A: ");
        double a = sc.nextDouble();
        System.out.print("Lado B: ");
        double b = sc.nextDouble();
        System.out.print("Lado C: ");
        double c = sc.nextDouble();
        boolean valido = (a + b > c) && (a + c > b) && (b + c > a);
        System.out.println(valido ? "Triângulo válido" : "Inválido");
        sc.close();
    }
}'

criar_java "LESM08" 'package luiseduardo;
import java.util.Scanner;
public class LESM08 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        final String USER = "admin";
        final String PASS = "1234";
        System.out.print("Usuário: ");
        String u = sc.next();
        System.out.print("Senha: ");
        String p = sc.next();
        System.out.println(USER.equals(u) && PASS.equals(p) ? "Login bem-sucedido" : "Login incorreto");
        sc.close();
    }
}'

criar_java "LESM09" 'package luiseduardo;
import java.util.Scanner;
import java.util.Arrays;
public class LESM09 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        double[] nums = new double[3];
        for (int i = 0; i < 3; i++) {
            System.out.print("Número " + (i+1) + ": ");
            nums[i] = sc.nextDouble();
        }
        Arrays.sort(nums);
        System.out.println("Ordem crescente: " + nums[0] + ", " + nums[1] + ", " + nums[2]);
        sc.close();
    }
}'

criar_java "LESM10" 'package luiseduardo;
import java.util.Scanner;
public class LESM10 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Ano: ");
        int ano = sc.nextInt();
        boolean bis = (ano % 400 == 0) || (ano % 4 == 0 && ano % 100 != 0);
        System.out.println(bis ? "Ano bissexto" : "Não é bissexto");
        sc.close();
    }
}'
