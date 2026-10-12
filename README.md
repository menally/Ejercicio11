import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Ingresa la longitud del lado A: ");

        double a = sc.nextDouble();
        //double a, b, c: Guardan las longitudes de los tres lados//

        System.out.print("Ingresa la longitud del lado B: ");
        double b = sc.nextDouble();

        System.out.print("Ingresa la longitud del lado C: ");
        double c = sc.nextDouble();

        if ((a + b > c) && (a + c > b) && (b + c > a)) {
            //if: Comprueba si los lados cumplen las condiciones//
            //&&: Indica que todas las condiciones deben cumplirse//

            System.out.println("Resultado del análisis: ESTRUCTURA_VÁLIDA");
            //ESTRUCTURA_VÁLIDA:Se muestra si las condiciones se cumplen//

        } else {

            System.out.println("Resultado del análisis: ESTRUCTURA_INVÁLIDA");
            //ESTRUCTURA_INVÁLIDA: Se muestra si alguna condición no se cumple//
        }

        sc.close();
    }
}
//El programa solicita tres longitudes y comprueba si pueden formar una estructura
// válida de acuerdo con las condiciones establecidas.