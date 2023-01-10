# Modelo-de-agenda
import java.util.Scanner;

public class Agenda {
  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    String opcao;
    String nome;
    String telefone;
    String email;
    
    do {
      System.out.println("\nMenu:");
      System.out.println("1 - Inserir contato");
      System.out.println("2 - Remover contato");
      System.out.println("3 - Atualizar contato");
      System.out.println("4 - Listar contatos");
      System.out.println("0 - Sair");
      
      opcao = scanner.nextLine();
      
      switch (opcao) {
        case "1":
          System.out.println("\nInserir contato:");
          System.out.print("Nome: ");
          nome = scanner.nextLine();
          System.out.print("Telefone: ");
          telefone = scanner.nextLine();
          System.out.print("Email: ");
          email = scanner.nextLine();
          // Aqui você pode inserir os dados de contato em um banco de dados ou em uma estrutura de dados (como um ArrayList)
          break;
        case "2":
          System.out.println("\nRemover contato:");
          System.out.print("Nome: ");
          nome = scanner.nextLine();
          // Aqui você pode remover o contato com o nome especificado de um banco de dados ou de uma estrutura de dados
          break;
        case "3":
          System.out.println("\nAtualizar contato:");
          System.out.print("Nome: ");
          nome = scanner.nextLine();
          System.out.print("Telefone: ");
          telefone = scanner.nextLine();
          System.out.print("Email: ");
          email = scanner.nextLine();
          // Aqui você pode atualizar os dados de contato de um contato com o nome especificado em um banco de dados ou em uma estrutura de dados
          break;
        case "4":
          System.out.println("\nListar contatos:");
          // Aqui você pode listar todos os contatos armazenados em um banco de dados ou em uma estrutura de dados
          break;
        case "0":
          System.out.println("Saindo...");
          break;
        default:
          System.out.println("Opção inválida!");
      }
    } while (!opcao.equals("0"));
  }
}



