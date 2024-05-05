# javacontador

ublic class contador {
    private int valor;

    // Construtor para inicializar o contador com um valor inicial

    public contador(int valorInicial) {
        this.valor = valorInicial;
    }
    // Método para incrementar o contador
    public void incrementar() {
        this.valor++;
    }

    // Método para decrementar o contador
    public void decrementar() {
        if (this.valor > 0) {
            this.valor--;
        } else {
            System.out.println("o contador já está em zero. Não é possível decrementar mais.");
        }
    }

    // Método para obter o valor atual do contador
    public int getValor() {
        return this.valor;
    }

    public static void main(String[] args) {
        // Criando uma instância do contador com valor inicial de 0
        contador meuContador = new contador(0);

        // Incrementando o contador algumas vezes
        meuContador.incrementar();
        meuContador.incrementar();
        meuContador.incrementar();

        // Imprimindo o valor atual do contador
        System.out.println ("Valor do contador: " + meuContador.getValor());

        // Decrementando o contador algumas vezes
        meuContador.decrementar();
        meuContador.decrementar();

        // Imprimindo o valor atual do contador novamente
        System.out.println("Valor do contador após decremento: " + meuContador.getValor());
    }
}
