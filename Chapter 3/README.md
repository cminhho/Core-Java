# Java Class & Object
Class is a template for creating objects which defines its state and behavior. A class contains field and mothod to difine the state and bahavior of its object.

#### Syntax for Declaring Class
```
<Access Modifier> class <Class_Name> extends <Super_Class_Name> implements <Interface_Name>
```
**Access modifier** defines who in java world can access the class and the members of the class
**Class_Name** Unique name for the class in a specific package.
**Interface_Name** Name of an Interface which the above class implements

#### Internal structure of Class
```
<Access Modifier> class <Class_Name> extends <Super_Class_Name> implements <Interface_Name>{
    <static initilizar block>
    <ananymous block>
    <constructor declarations>
    <field declarations (Static and Non-Static)>
    <method declarations (Static and Non-Static)>
    <Inner class declarations>
    <nested interface declarations>
    Access variables inside class
}
```

#### Example of Java Class
```
package com.cminhho;

import java.lang.*;

public class TestClass {
  public int i;
  static {
    System.out.println("This is static block");
  }

  {
    System.out.println("This is ananuymous block");
  }

  TestClass(){
    System.out.println("This is constructor");
  }

  void method(){
    System.out.println("This is method");
  }
  public static void main(String args[]){
	  System.out.println("This is main method");
  }
}
class AnotherClass {
}
```
Classes are writen in a java source file. A source file can contain more than one java class 

#### Rules applied to Source code file
- There can be only one public class per source code file but can have multiple non public classed.
- In case there is any public class persent in the source file, name of the file should be the name of the class.
- Sequence of statements in source code file should be package >> import >> Class declaration.
- No sequence rule is applied for Comments. Comment can be there in any part of the source code file at any location.
- Files with no public class can have any name for the class, there is no rule for the same 
- **Import and package** statements should be applied to all classed in the same source code file.

#### How to Create an Object of Class
To create object of a class **<new> Keyword** can be used
*Syntac*
```
<Class_Name> ClassObjectReference = new <Class_Name>();
```
Here constructor of the class(Class_Name) will get executed and object will be created 

#### How to Access Member of a Class
You can call method of an object by naming followed any a period, this should be flolowed by the name of the method and its argumant list
```
 objectName.methodName(arg1, arg2, arg3).
```

### Bullet Points
* Class can have only public and defautl access
* Public class needs to be in same name java file.
* Single java file can contain more then one non public class but can have only one public class
* A public class can be seen by all classed from all package.
* A class with default access can be seen only by classes within the same package.
* Java file with no public class have no naming restriction.
* Class can also have final and abstract & strictfp non access modifiers.
* An abstract class can not be initiated.
* A final class can not be subclassed.
* A class can not be both final and abstract.
* Class visibility can be seen in 3 parameter.
