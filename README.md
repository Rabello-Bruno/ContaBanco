codigo
.
.
.
.
.
.
.
.
.
import java.util.Scanner;

public class ContaTerminal {
    public static void main(String[] args) {
        // Criação do Scanner para ler a entrada do usuário
        Scanner scanner = new Scanner(System.in);
        
        // Solicita e lê o número da agência
        System.out.println("Por favor, digite o número da Agência:");
        String agencia = scanner.nextLine();
        
        // Solicita e lê o número da conta
        System.out.println("Por favor, digite o número da Conta:");
        int numero = scanner.nextInt();
        scanner.nextLine();  // Limpa o buffer do scanner
        
        // Fechando o scanner
        scanner.close();
        
        // Simulação de um saldo armazenado
        double saldo = obterSaldo(agencia, numero);
        
        // Exibe a mensagem formatada com as informações do usuário
        System.out.println("Olá, obrigado por criar uma conta em nosso banco. Sua agência é " + 
                           agencia + ", conta " + numero + " e seu saldo de R$ " + saldo + " já está disponível para saque.");
    }
    
    // Método que simula a obtenção do saldo a partir da agência e número da conta
    private static double obterSaldo(String agencia, int numero) {
        // Aqui podemos adicionar lógica para obter o saldo real de um banco de dados
        // Para o exemplo, vamos retornar um saldo fixo.
        return 237.48;
    }
}
