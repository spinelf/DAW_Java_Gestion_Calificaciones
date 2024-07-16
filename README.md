![ActividadEvaluacion-4](https://github.com/user-attachments/assets/c34571fb-3cec-41c9-9699-c9af8ea56e0b)

## Enunciado

Esta práctica consiste en la elaboración de un proyecto en Eclipse para gestionar las calificaciones de los alumnos en un centro de enseñanza.

Debes crear un proyecto en Eclipse con el nombre EjercicioUF7-01 atendiendo a las especificaciones que se indican en este documento.
Empaquetarás el proyecto en un archivo .zip que entregarás a tu tutor junto con un documento en formato Word o PDF donde realizarás una exposición sobre lo que has ido realizando y pegarás las partes principales del código.
Especificaciones

Para resolver el problema propuesto crearás la clase Alumno como compuesto, cuyos componentes son: nombre, matricula y calificaciones, siendo calificaciones un objeto ArrayList de objetos de tipo Calificacion.
Debes terminar de implementar la clase Calificacion completando el código que falta en la posición de los comentarios:

    public class Calificacion {

              private String asignatura;

              private int nota; // Valor de 0 a 100

              // Constructor que reciba argumentos para las dos propiedades

            // Métodos get/set

            @Override

            public String toString() {

                                // Devolver una cadena de tipo: “Lengua: 55”

            }

    }

Debes terminar de implementar la clase Alumno completando el código que falta en la posición de los comentarios:
import java.util.ArrayList;

    public class Alumno {

              private String nombre;

              private int matricula;

              private ArrayList<Calificacion> calificaciones;

              public Alumno(String nombre, int matricula) {

                           // Asignar a las propiedades nombre y matricula

                          // los valores de los parámetros.

                         // Construir objeto ArrayList calificaciones.

              }

             // Añadir métodos get para las tres propiedades

            // que serán de solo lectura.

           public void calificar(String asignatura, int nota) {

                        // Añadir la nueva calificación

                       // a la colección de calificaciones.

           }

           @Override

           public String toString() {

                        // Devolver una cadena similar a la de este ejemplo:

                       // “Alumno matricula: 31553 - Carmen Torres”

           }

    }

En una clase Principal, dentro del método main, debes crear un objeto Alumno, añadirle 6 calificaciones y luego mostrar en pantalla los datos del alumno, el listado de calificaciones y la nota media. La salida en pantalla una vez ejecutado el programa será algo así:

    Alumno matrícula: 31553 - Carmen Torres
    Matemáticas: 70
    Lengua: 55
    Inglés: 93
    Física: 82
    Educación física: 82
    Biología y geología: 58
    NOTA MEDIA: 73
