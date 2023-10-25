import java.util.HashMap;

public class LineaDeTiempoColombia {
    public static void main(String[] args) {
        HashMap<String, String> nombres = new HashMap<>();
        HashMap<String, String> formasDeGobierno = new HashMap<>();
        HashMap<String, String> constituciones = new HashMap<>();
        HashMap<String, String[]> caracteristicas = new HashMap<>();

        // Llenar los datos
        nombres.put("Virreinato del Peru", "1542-1717");
        formasDeGobierno.put("Virreinato del Peru", "Colonización española");
        constituciones.put("Virreinato del Peru", "No había una constitución propia");
        caracteristicas.put("Virreinato del Peru", new String[] {
            "Explotación de recursos naturales",
            "Dominio de la población indígena"
        });

        // Agregar más datos para otros períodos históricos...

        // Imprimir la línea de tiempo
        for (String nombre : nombres.keySet()) {
            System.out.println("Nombre: " + nombre);
            System.out.println("Fechas: " + nombres.get(nombre));
            System.out.println("Forma de Gobierno: " + formasDeGobierno.get(nombre));
            System.out.println("Constitución Política: " + constituciones.get(nombre));

            String[] caracteristicasPeriodo = caracteristicas.get(nombre);
            System.out.println("Características:");
            for (String caracteristica : caracteristicasPeriodo) {
                System.out.println("- " + caracteristica);
            }

            System.out.println(); // Separador
        }
    }
}
