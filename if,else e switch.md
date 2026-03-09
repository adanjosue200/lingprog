import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner teclado = new Scanner(System.in);

        int codigo;
        int idade;
        double preco = 0;
        double precoFinal;

        // menu
        System.out.println("Menu Java Lanches");
        System.out.println("101 - Cachorro Quente (R$10)");
        System.out.println("102 - X-Burger (R$15)");
        System.out.println("103 - X-Salada (R$12)");

        System.out.print("Digite o codigo do produto: ");
        codigo = teclado.nextInt();

        // produto
        switch(codigo) {
            case 101:
                preco = 10;
                break;

            case 102:
                preco = 15;
                break;

            case 103:
                preco = 12;
                break;

            default:
                System.out.println("Produto invalido");
                return; // termina o programa
        }

        // idade
        System.out.print("Digite sua idade: ");
        idade = teclado.nextInt();

        // desconto
        if (idade < 12) {
            precoFinal = preco * 0.5; // 50% desconto
        }
        else if (idade <= 60) {
            precoFinal = preco; // sem desconto
        }
        else {
            precoFinal = preco * 0.7; // 30% desconto
        }

        // resultado
        System.out.println("Preco final: R$ " + precoFinal);
    }
}
