# java-master-class-notes

Java Master class note:

Installing java for windows:

installing Amazon correto(JDK for windows )

1.Default whole number used by java is int.int is recommended for whole numbers.
byte byyeDiviedByIntValue = (int)(maxByteValue/2);// typecasted to remove compilation error.

2.By default floating point numbers are treated as double by default.
double is recommended for floating point numbers.
float floatValue=4.4;//Will give compilation error if we dont put "f" or typecast to float.

3.Why use of double is recommended:
  firstly,
  Computers have at cheap level functionality to process double numbers faster than their equivalent float numbers.
  
  secondly,
  Its precise ,that's why most of libraries use double internally. 
 
4.Why floating point numbers(float or double) are not used for example currency calculations ?
Because of the way they stored in the memory.We dont use them for currency calculations.

Solution: use BigDecimal for currency calculations.

5.Switch statements work with ints,chars, and Strings

6.You can create object using default construtor with some default value.
//Call any parameterized construtor with default values i.e this("firstName","lastName");

public Person(){
	this("firstName","lastName");
}

7.Dont call any method inside the construtor.
Reason being method call might fail due any reason.Also goal of methods is work on ready-made object rather than creating objects.

8.Constructor chaining to duplicate the code.

9.Subclass only inherits members(instance variables, methods and nested classed).Since
construtors are not member of the class they are not inherited.

10.Overloading does not anything to do polymorphism But Java developers refer to it as compile time polymorphism.
We can overload static and instance methods

11.Overloading usually happens in a single class but in case of subclasses we can have scenario of overloading.

12.Method overloading rules:
Must have:
	#same method name
	#diffent parameters

May or may not have:
