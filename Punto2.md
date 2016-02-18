# Punto2
Laboratorio 1 punto 2 Aplicaciones Moviles

Abstracción

La abstraccion es el proceso de ocultar los detalles de la implementación al usuario, solo la funcionalidad sera entregada al usuario.
Es decir que el usuario tendra la informacion sobre que hace un objeto pero no de como lo hace. En java se logra la abstraccipon por medio de Intefaces y clases abstract.

Interfaz

Una interfaz es un tipo de referencia en java (similar a una clase), es una coleccion de methodos abstract  Una clase que implemente una interface hereda los metodos abstract de la interfaz. Las intefaces se describen de la misma manera que las clases, pero las clases describen los atributos y comportamientos del objeto a diferencia de la interfaz que contiene el comportamiento que la clase implementa.

Ejemplo:

interface Animal {

   public void eat();
   public void travel();
}

public class MammalInt implements Animal{

   public void eat(){
      System.out.println("Mammal eats");
   }

   public void travel(){
      System.out.println("Mammal travels");
   } 

   public int noOfLegs(){
      return 0;
   }

   public static void main(String args[]){
      MammalInt m = new MammalInt();
      m.eat();
      m.travel();
   }
} 

Abstract

Las clases asbtract son clases que no pueden ser inicializadas, es decir que no se pueden crear instancias de una clase abstract. Estas clases tienen como proposito servir como base para subclases que se hereden de esta.

Ejemplo

abstract class Animal {

  public void eat(){
      System.out.println("Mammal eats");
   }
   public void travel();
}

public class MammalInt extends Animal{

  public void travel(){
      System.out.println("Mammal travels");
   } 

  public static void main(String args[]){
      MammalInt m = new MammalInt();
      m.eat();
      m.travel();
   }
} 





