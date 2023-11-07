import java.util.ArrayList;
import java.util.List;
import java.util.Locale;
import java.util.Scanner;

public class Ex05_Listas {
    public static void main(String[] args) {
        Locale.setDefault(Locale.US);
        Scanner sc = new Scanner(System.in);

        // CRIAÇÃO DAS LISTAS
        List<String> nomes = new ArrayList<>();
        List<Integer> Ids = new ArrayList<>();
        List<Double> salary = new ArrayList<>();

        System.out.print("Quantas pessoas serão? ");
        int n = sc.nextInt();

        // IMPLEMENTANDO UM NOVO VALOR NA LISTA.
        for (int number = 0; number < n; number++) {
            System.out.println(" ");
            System.out.println("Empregado #" + (number + 1));
            System.out.print("Nome: ");
            String name = sc.next();
            nomes.add(name);

            System.out.print("ID: ");
            int ids = sc.nextInt();
            Ids.add(ids);

            System.out.print("Salário: ");
            double salario = sc.nextDouble();
            salary.add(salario);
        }
        // PARTE 2
        System.out.println(" ");
        System.out.println("====================================================");
        System.out.println("IMPLEMENTAÇÃO DE FUNCIONÁRIOS FOI FEITA COM SUCESSO");
        System.out.println("====================================================");
        System.out.println(" ");

        // TRATAMENTO DO ERRO
        System.out.print("Me diga por ID qual funcionário receberá o bônus: ");

        while (true) {

            int ids_search = sc.nextInt();
            var resultados = Ids.indexOf(ids_search);

            if (resultados == -1) {
                System.out.println("ID N ENCONTRADO");
                System.out.print("Digite novamente: ");

            } else {
                System.out.print("Quantos porcento? ");
                int percent = sc.nextInt();
                System.out.println("LISTA DE EMPREGADOS");
                for (int i = 0; i < n; i++) {
                    System.out.println(Ids.get(i) + "," + nomes.get(i) + "," + (((salary.get(i) * percent) / 100) + salary.get(i)));
                }
                break;
            }

        }


    }
}
