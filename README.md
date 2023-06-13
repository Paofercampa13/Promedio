# Promedio
Promedio 
public class Main {

    public static void main(String[] args) {
        Scanner teclado = new Scanner(System.in);
        double Calificacion1, Calificacion2, Calificacion3, Calificacion4, Calificacion5, promedio;
        String Alumno;

        System.out.println("Nombre del Alumno: ");
        Alumno = teclado.nextLine();
        System.out.println("Calificacion de Matematicas: ");
        Calificacion1 = teclado.nextDouble();
        System.out.println("Calificacion de Español: ");
        Calificacion2 = teclado.nextDouble();
        System.out.println("Calificacion de Ingles: ");
        Calificacion3 = teclado.nextDouble();
        System.out.println("Calificacion de Deportes: ");
        Calificacion4 = teclado.nextDouble();
        System.out.println("Calificacion de Danza: ");
        Calificacion5 = teclado.nextDouble();
        promedio = (Calificacion1 + Calificacion2 + Calificacion3 + Calificacion4 + Calificacion5) / 5;
        char resultado = obtenerCaracterPromedio(promedio);

        System.out.println("Promedio Final: " + promedio);
        System.out.println("Caracter correspondiente al promedio: " + resultado);
    }

    public static char obtenerCaracterPromedio(double promedio) {
        if (promedio >= 51) {
            return 'F';
        } else if (promedio >= 61) {
            return 'E';
        } else if (promedio >= 70) {
            return 'D';
        } else if (promedio >= 80) {
            return 'C';
        } else if (promedio >= 90) {
            return 'B';
        } else {
            return 'A';
        }
    }
}
