# Java8LamdaBasics

Below are some basic notes 

Lambda Basics 

OOPS shortcomings

1)Everything is an oject 
2)All code blocks are associated with classes and objects

rather then passing a behaviour(Class) lambda are made to pass an action(Method without class) 
assign a block of code aas vlue to a variable in java > we can do it using lambd
in lambda exp we implement the method of an inteface(functional only) directy without implemeting it using a class


------------
on high level we can say that lambda expressions are shortcut to anonymous inner class but technicall its not a correct statement (actually both are diffrent things) they just look similar 

typeinferance in lamda -> while passing arguments in a lambda exp we dont need to mention its type as the compiler themselves mathes the type with the mapped interface --this is called type inferance in lambda expressions 
compiler infers 
a)what the input type is 
waht is return type 

Functional Interface -> an interface with only one abstract method (remember form java 8 onwards interface can have implemented methds as well(of static and default type)


Exception handling in lambda is done by wrapping the lambda into other lambda, or by using try catch in lambda itself 

clousers in java -> the concet of effectively final valriables comes into picture here 

how lambda and Anonymous inner class are diffrent ->"this" refrence refers to instance of an anonymous inner class in case of an  lambda it does not overrides it still refers to the conteext of the main method in which lambda is present.


Method refrences in lambda -> 

//printConditionally(people, p -> true, p -> System.out.println(p));
		//above method call can alternatively done by method reference as well 
		printConditionally(people, p -> true, System.out::println);
		
or 

	Thread myThread = new Thread(() -> print());
		myThread.run();
		
		//same thing can be done using methodRefrence 
		Thread myThreadMethodRefrence = new Thread(MethodRefrenceExample1::print);
		myThreadMethodRefrence.run();
		
For Each in java 8  -->Extrenal iterator (normal for loop or foreach/for-in loop)
**consumer is a functional iterface that comes with java 8 

=--------------------------------========================-----------------------------------------=====

Stream - a sequence of elements supporting sequential and paralelaggregation operation 





 

 
