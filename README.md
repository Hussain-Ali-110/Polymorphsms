# Polymorphsms
 
package polymorphisms;

 
 // @author TAHIR ALI 
 
// Superclass
class Animal {

    public void sound() {
        System.out.println("Animal makes a sound");
    }
}

// Subclass Dog
class Dog extends Animal {

    @Override
    public void sound() {
        System.out.println("Dog barks");
    }
}

// Subclass Cat
class Cat extends Animal {

    @Override
    public void sound() {
        System.out.println("Cat meows");
    }
}

// Main class to test polymorphism
public class Main {

    public static void main(String[] args) {
        Animal myAnimal;  // Declare an Animal reference

        // Assign Dog object to Animal reference
        myAnimal = new Dog();
        myAnimal.sound(); // Outputs: Dog barks

        // Assign Cat object to Animal reference
        myAnimal = new Cat();
        myAnimal.sound(); // Outputs: Cat meows
    }
}

