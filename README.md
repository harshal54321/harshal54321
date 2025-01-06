A]   Single Inheritance :
 
Program :
 
package vehicle; class Car {
String brand="Ford"; public void display(){
System.out.println("Hello Ford!");
 
}
 
}
 
class Vehicle extends Car {
 
String Model_name="Mustang";
 
 
public static void main(String[] args) { Vehicle c=new Vehicle(); c.display();
System.out.println(c.brand+" "+c.Model_name);
 
}
 
}



A]  Multilevel Inhritance : Program :
package multilevel; class Animal {
void eat(){ System.out.println("Eating... ");
}
 
}
 
class Dog extends Animal { void bark(){
System.out.println("Barking .. ");
 
}
 
}
 
class BabyDog extends Dog { void weep(){
System.out.println("Weeping.. ");
 
}
 
}
 
public class Multilevel {
 
public static void main(String[] args) {

BabyDog d= new BabyDog(); d.weep();
d.bark();
 
d.eat();
 
}
 
}
 

