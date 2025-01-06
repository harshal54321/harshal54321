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


A]	Super keyword : Pogram :
package pkgsuper; class Vehicle {
int maxspeed=120;
}


class Car extends Vehicle{ int maxspeed=180;
void display(){
System.out.println("Max Speed Is: "+super.maxspeed);
}
}


public class Super {
public static void main(String[] args) { Car c=new Car();
c.display();
}
}
 

B]	this keyword : Program :
package pkgthis; public class This {
int id=25;
String name="Sudha";


void display(int id,String name){ this.id=id;
this.name=name;
}
void show(){
System.out.println("ID:"+id+ " And "+"Name:"+name);
}


public static void main(String[] args) { This t=new This();
t.show();
}
}
 


C]	final Keyword :

Program :

package pkgfinal; public class Final { final int id=10;

void display(){ System.out.println("Student ID:"+id);
}


public static void main(String[] args) { Final obj=new Final(); obj.display();
obj.id=25; System.out.println(obj.id);
}
}


package innerclass;
public class MemberInner { private final int age=20;

class InnerClass{ void msg(){
System.out.println("Age is :- " + age);
}
}
public static void main(String[] args) { MemberInner obj=new MemberInner(); MemberInner.InnerClass in=obj.new InnerClass(); in.msg();

}
}


B]	Multithreading : Program :
package multithreding;


class MultithreadingDemo extends Thread { public void run()
{
try {
// Displaying the thread that is running System.out.println(
"Thread " + Thread.currentThread().getId()
+ " is running");
}
catch (Exception e) {
// Throwing an exception System.out.println("Exception is caught");
}
}
}
public class Multithread {


public static void main(String[] args) { int n = 8; // Number of threads
for (int i = 0; i < n; i++) {
MultithreadingDemo object = new MultithreadingDemo(); object.start();
}
}
}
 
Output :



C]	File Handling :
Program :
package exception;


public class Exception {
public static void main(String args[]){ try{
int data=100/0;
}catch(ArithmeticException e){ System.out.println(e);
}
System.out.println("Finish it...");
}
}
Output :



