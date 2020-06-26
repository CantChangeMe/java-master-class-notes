# java-master-class-notes


Installing java for windows:

installing Amazon correto(JDK for windows )

<pre>
1.Default whole number used by java is int.int is recommended for whole numbers.
byte byyeDiviedByIntValue = (int)(maxByteValue/2);// typecasted to remove compilation error.
</pre>
<pre>
2.By default floating point numbers are treated as double by default.
double is recommended for floating point numbers.
float floatValue=4.4;//Will give compilation error if we dont put "f" or typecast to float.
</pre>
<pre>
3.Why use of double is recommended:
  firstly,
  Computers have at cheap level functionality to process double numbers faster than their equivalent float numbers.
  
  secondly,
  Its precise ,that's why most of libraries use double internally. 
</pre>
<pre> 
4.Why floating point numbers(float or double) are not used for example currency calculations ?
Because of the way they stored in the memory.We dont use them for currency calculations.

Solution: use BigDecimal for currency calculations.
</pre>
<pre>
5.Switch statements work with ints,chars, and Strings
</pre>
<pre>
6.You can create object using default construtor with some default value.
//Call any parameterized construtor with default values i.e this("firstName","lastName");

public Person(){
	this("firstName","lastName");
}
</pre>
<pre>
7.Dont call any method inside the construtor.
Reason being method call might fail due any reason.Also goal of methods is work on ready-made object rather than creating objects.
</pre>
<pre>
8.Constructor chaining to duplicate the code.
</pre>
<pre>
9.Subclass only inherits members(instance variables, methods and nested classed).Since
construtors are not member of the class they are not inherited.
</pre>
<pre>
10.Overloading does not anything to do polymorphism But Java developers refer to it as compile time polymorphism.
We can overload static and instance methods
</pre>
<pre>
11.Overloading usually happens in a single class but in case of subclasses we can have scenario of overloading.
</pre>
<pre>
12.Method overloading rules:
Must have:
<pre>
	same method name
	diffent parameters
</pre>
May or may not have:
	1.different return types
	2.different accesss modifiers
	3.throw different checked or unchecked exception. 
</pre>
<pre>
13:Method overriding also known as runtime polymorphism or dyanamic method dispatch because method to be invoked is decided at runtime by JVM.
Best practice to use @Override so that compiler can throw error if overriding rules are followed.
</pre>
<pre>
14.Cant override static methods only instace methods can be overridden.
</pre>
<pre> 
15.Method overriding rules:
	1.Must have same name and arguments.
	2.Return type must be subclass of parent class method.
	3.Can not have lower access modifier. 
</pre>

16.Few points related to overriding to keep in mind:

	1.Only inherited methods can be overridden.
	2.Constructors and private methods can not be overridden.
	3.Final methods can not be overridden.
	4.A subclass can call superclass version of overridden method.
	i.e. super.getName();






