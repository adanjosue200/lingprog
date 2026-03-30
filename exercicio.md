import java.util.Scanner;

public class Ex1 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        String[] nomes = new String[5];

        for (int i = 0; i < 5; i++) {
            System.out.print("Digite um nome: ");
            nomes[i] = sc.nextLine();
        }

        System.out.println("Ordem inversa:");
        for (int i = 4; i >= 0; i--) {
            System.out.println(nomes[i]);
        }
    }
}
