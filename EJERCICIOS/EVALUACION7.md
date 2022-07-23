# 7. PROGRAMACIÓN ORIENTADA A OBJETOS (POO)
Objetivo: Verificar el dominio teórico y técnico del paradigma programación orientada a
objetos, mediante ejercicios para desarrollar su código y preguntas de respuesta
múltiple.

Indicaciones: Pedir responder cada una de las preguntas de manera acertada, breve y
clara, según sea el caso.

1. La Programación Orientada a Objetos es: (Valor 1 punto)

        c. Un paradigma que se basa en el uso de objetos.
      
2. Se refieren a características principalmente físicas y de estado de un objeto: (Valor 1 punto)

        b. Atributos

3. Sirve para derivar de una clase ya existente a otra clase: (Valor 1 punto)

        a. Herencia
        
4. De las siguientes opciones, selecciona las ventajas de la Programación Orientada a Objetos: (Valor 1 punto)


        b. Simplicidad

        d. Reutilización de código
        
5. Las clases normalmente cuentan con: (Valor 1 punto)

        c. Nombre de clase, atributos y métodos.
        
6. En programación, se utiliza para modelar un conjunto de objetos: (Valor 1 punto)

        b. Clase
        
7. ¿Qué son los métodos?

        b. Las operaciones realizables de un objeto.
        
8. Identifica las partes de una clase:

![image](https://user-images.githubusercontent.com/104698382/180622907-a8649f52-43fd-46ff-baac-5de6d8435a0a.png)

9. Deberás crear un programa que forme parte de un módulo para el sistema de una
estética de perros. El programa deberá de contener lo siguiente: (Valor 2 puntos)

a. Una clase RecibeMascota.

b. Los atributos: nombre de perro, edad, raza, tamaño y nombre de dueño.

c. Crear el método main en donde contendrá el código para realizar el
siguiente procedimiento:

  i. Crear un arreglo dinámico de tipo de la clase.
  
  ii. Hacer una instancia para crear un objeto de tipo de la clase.
  
  iii. Asignar valores a los atributos de la clase con datos que tú prefieras.
  
  iv. Agregar el objeto creado al arreglo.
  
  v. Imprimir la cantidad de perros que se encuentran en la estética con el
  siguiente mensaje: Perros actuales en la estética: “Número de
  perros”.

                import java.util.ArrayList;
                  public class RecibeMascota {
                      String nombre; // Nombre de la mascota
                      int edad; // Edad de la mascota
                      String raza; // raza de la mascota
                      double tamano; // tamanio de la mascota
                      String nombreDueno; // Nombre completo del duenio
                      public static void main(String args[]) {
                        // Creamos un arreglo de tipo RecibeMascota
                          ArrayList<RecibeMascota> mascotasActuales = new ArrayList();

                          // Hacemos una instancia y creamos un objeto de tipo RecibeMascota
                          RecibeMascota miManada = new RecibeMascota();
                          miManada.nombre = "doggy";
                          miManada.edad = 18;
                          miManada.raza = "pug";
                          miManada.tamano = 0.8;
                          miManada.nombreDueno = "Monserrat Lopez";
                          mascotasActuales.add(miManada);
                          System.out.println("Perros actuales en la estetica: " + mascotasActuales.size());
                      }

                  }
