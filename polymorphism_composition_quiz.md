# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Polymorphism means 'many forms'.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

When applied to OO design it means that an object has the ability to take on many forms, or it can be an instance of multiple classes at the same time. For example, Student class is a child of Person class, the polymorphism occurs when a parent class reference is used to refer to a child class object.

Student student = new Student()
Person person = new Student()


3. What can we use to implement polymorphism in Java?

Polymorphism can be implemented by using inheritance or interfaces.

4. How many 'forms' can an object take when using polymorphism?

In case of inheritance only object will have its parent form as well as its own.
In interfaces, it depends on the number of implemented interfaces.

5. Give an example of when you could use polymorphism.

Polymorphism can be used when there are many methods with the same name and doing the same thing but for different Class types. Rather than recreating the same method for each class, interface can be created and then each new class implements that interface. In that way the code becomes more DRY and reusable.  




# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

Composition in OOP context means that an object is composed or made up of other objects and it also holds ownership of those objects. In other words, when this object is destroyed all objects that composed it are destroyed too.

7. When would you use composition? Provide a simple example in Java.

Composition should be used when objects composing another object cannot live indpendently.

For example,

public class Computer {
  private Processor processor;
  ...

}

public class StandardProcessor implements Processor {
  private String model;
}


8. Give a difference between composition and aggregation?

The difference between the two is that in aggregation the objects can live independently.

9. What is/are the advantage(s) of using composition/aggregation?

The main adventage of using composition/aggregation is that it offers more flexibility over
inheritance as it is easier to build classes out of various components rather than trying to find commonalities between them and creating a family tree.

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

All these objects are destroyed too.

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

They remain independently intact. 
