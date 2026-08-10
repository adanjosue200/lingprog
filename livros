public class livros {


    private static int totalLivros = 0;

    // Atributos
    private String titulo;
    private String autor;
    private boolean disponivel;


    public livros(String titulo, String autor) {
        this.titulo = titulo;
        this.autor = autor;
        this.disponivel = true;

        totalLivros++;
    }


    public livros(String titulo, String autor, boolean disponivel) {
        this.titulo = titulo;
        this.autor = autor;
        this.disponivel = disponivel;

        totalLivros++;
    }


    public static int getTotallivros() {
        return totalLivros;
    }


    public void emprestar() {
        if (disponivel) {
            disponivel = false;
            System.out.println("Livro \"" + titulo + "\" foi emprestado.");
        } else {
            System.out.println("O livro \"" + titulo + "\" já está emprestado.");
        }
    }

    public void devolver() {
        disponivel = true;
        System.out.println("Livro \"" + titulo + "\" foi devolvido.");
    }


    public void exibirFicha() {
        System.out.println("Ficha do Livro -----");
        System.out.println("Título: " + titulo);
        System.out.println("Autor: " + autor);

        if (disponivel) {
            System.out.println("Status: Disponível");
        } else {
            System.out.println("Status: Emprestado");
        }

        System.out.println();
    }
