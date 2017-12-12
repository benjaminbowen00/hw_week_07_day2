# Polymorphism & Composition Homework - Quiz

# Polymorphism

#In class example it is not the interface that makes the polymorphism - it is the ability to label an object by a class above it but it still holds the information that it is from the subclass.
#Inheritance implies Polymorphism but we can also get polymorphism from implementing an interface.

1. What does the word 'polymorphism' mean?
It means it is possible for an object to take different forms - it could behave as if it is from the parent class or the child class.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.
We can use a parent class reference and actually refer to the child class.
It means if we have a method that is of the same name in the superclass and the parent class, we can treat the object as if it is from the superclass but can still access the methods from the child class. It can take the form of the superclass in a collection but the child class when a method is called.
E.g. Animal class which has method roar - returns 'roar'
    Cat extends animal and has method roar - returns 'meow'
    Dog extends animal and has method roar - returns 'woof'
We can make an arrayList of animal objects - if we put in an animal, a cat and a dog then get each to roar, they would each return different things.


3. What can we use to implement polymorphism in Java?
We can use superclasses or interfaces to group things together.

4. How many 'forms' can an object take when using polymorphism?
As many different parent classes or interfaces to which it belongs.

5. Give an example of when you could use polymorphism.
If you want to group objects in an arraylist, they need to be of the same type. Objects from different subclasses but the same superclass could therefore be in an arraylist together. The object have different behaviour based on the which form it takes.
E.g. tv and mobile phone both might inherit from a screen superclass. Both could have a start up and shutdown method but these can be different. We could make a collection of screens that include tvs and mobile phones but the method they use for starting up/shutting down would be different.


# Composition

#From example - it is not the IOutput that makes the composition but that the computer has an (any) output device that has its own methods which can be utilised by the computer.

6. What do we mean by 'composition' in reference to object-oriented programming?
It is when a class has another class (or interface) as a field or is included in one of its attributes.

7. When would you use composition? Provide a simple example in Java.
When one class is not a super/subclass of another but you would like to use its methods.
E.g. A car has an engine (engine is not a subclass of car), so an engine is a component of car and the car can use the start method so that the car starts.

8. What is/are the advantage(s) of using composition?
You can choose which methods from the composed part to expose and use - you don't automatically get them all like in inheritance.
An object can be composed of many parts but multiple inheritance is not possible.hip.
All the associated information that comes with inheritance may not be wanted - if there is no superclass-subclass relations

9. What happens to the behaviours when the object composed of them is destroyed?
The behaviours are also destroyed.
