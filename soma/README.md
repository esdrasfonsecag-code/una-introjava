# ⚡ Exercício 2: Subtração, Multiplicação e Divisão - Java

**Localização do arquivo:** [operacoes/Main.java](operacoes/Main.java)

---

## 📝 Descrição
Programa em Java que lê **dois números inteiros** informados pelo usuário e realiza as seguintes operações:  

- 🔹 **Subtração** do primeiro pelo segundo  
- 🔹 **Multiplicação** do primeiro pelo segundo  
- 🔹 **Divisão** do primeiro pelo segundo (com verificação para evitar divisão por zero)  

---

## 💻 Código completo

```java
import java.util.Scanner;

public class Main {
  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.print("Digite o primeiro numero: ");
    int num1 = sc.nextInt(); 

    System.out.print("Digite o segundo numero: ");
    int num2 = sc.nextInt();

    int subtracao = num1 - num2;
    int multiplicacao = num1 * num2;

    if (num2 != 0) {
      double divisao = (double) num1 / num2;
      System.out.println("Divisao: " + divisao);
    } else {
      System.out.println("Divisao: nao e possivel dividir por zero");
    }

    System.out.println("Subtracao: " + subtracao);
    System.out.println("Multiplicacao: " + multiplicacao);

    sc.close();
  }
}

