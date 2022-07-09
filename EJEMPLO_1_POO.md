 Creación de una clase con atributos y metodos
 
    public class Usuario{
        //Atributos
        String nombre;
        String folio;

        //metodos
        public static void main(String[]args){
            Usuario usuario1=new Usuario();

            usuario1.nombre="David";
            usuario1.folio="A8484";
            System.out.println("El nombre del usuario es "+usuario1.nombre);
            System.out.println("El folio del usuario es "+usuario1.folio);

            Usuario usuario2=new Usuario();

            usuario2.nombre="Pedro";
            usuario2.folio="B8459";
            System.out.println("El nombre del usuario es "+usuario2.nombre);
            System.out.println("El folio del usuario es "+usuario2.folio);
        }
    }



      public class Usuario{
          //Atributos
          String nombre;
          String folio;

          //metodo para pedir los datos
          Scanner in = new Scanner (System.in);	
          public void leerDatos(){
             System.out.println("Cual es el nombre del usuario?: ");
             nombre = in.nextLine();
             System.out.println("ingresa el folio del usuario");
             folio=in.nextLine();

            }
              //metodo para imprimir los datos
         public void muestraDatos(){
          System.out.println("El nombre del usuario es : "  + nombre);
              System.out.println("El folio del usuario es : "  + folio);


         }
          public static void main(String[]args){
              Usuario usuario1=new Usuario();
              usuario1.leerDatos();
              usuario1.muestraDatos();

         }

      }


MI PROGRAMA EN JAVA:

    // Online Java Compiler
    // Use this editor to write, compile and run your Java code online
    import java.util.Scanner;
    class Calculadora {
        //Atributos
        double num1 = 0, num2 = 0, res = 0;
    
    //metodo para pedir datos
    Scanner entrada = new Scanner(System.in);
    
    public void suma(){
        System.out.println("***Elegiste SUMA***");
        res = num1 + num2;
        System.out.println("El resultado de la suma de " + num1 + " mas " + num2 + " es igual a " + res);
    }
    
    public void resta(){
        System.out.println("***Elegiste RESTA***");
        res = num1 - num2;
        System.out.println("El resultado de la resta de " + num1 + " menos " + num2 + " es igual a " + res);
    }
    
    public void multiplicacion(){
        System.out.println("***Elegiste MULTIPLICACION***");
        res = num1 * num2;
        System.out.println("El resultado de la multiplicacion de " + num1 + " por " + num2 + " es igual a " + res);
    }
    
    public void division(){
        System.out.println("***Elegiste DIVISION***");
        res = num1 / num2;
        if (num2 == 0){
            System.out.println("SYNTAX ERROR!");
        } else {
            System.out.println("El resultado de la division de " + num1 + " entre " + num2 + " es igual a " + res);
        }
        
    }
    
    public void ingresarDatos(){
        System.out.println("Ingresa el primer numero: ");
        num1 = entrada.nextInt();
        System.out.println("ingresa el segundo numero");
        num2 = entrada.nextInt();
    }
    
    public void imprimirDatos(){
        System.out.println("El primer numero ingresado es: " + num1);
        System.out.println("El segundo numero ingresado es: " + num2);
    }
    
    public static void main(String[] args) {
        Calculadora operacion1 = new Calculadora();
        operacion1.ingresarDatos();
        operacion1.imprimirDatos();
        operacion1.suma();
        operacion1.resta();
        operacion1.multiplicacion();
        operacion1.division();
         
    }
}
