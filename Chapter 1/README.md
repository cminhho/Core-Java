# Getting Started with Java 
Here we will discuss some basics topics related to Java

#### How to Download Java
Lasted version of Java can be download from [Java Website](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)

#### Java Installation
Once java is downloaded, it can be installed like any other software (.exe) in your Windows system. 

#### Setting up the Environment Varibales
After installing Java there are some environment variables that need to be set.
 - CLASSPATH: This environment variable points the location of JDK home directory. It also contains the address of the folder from where the jars get loaded by the ClassLoader 
 - JAVA_HOME: This environment variable will point the location of JAva home directory
 
#### How to Check if Java is Installed 
To check if your Java is installed properly open Command Prompt. In the command prompt window wite **"java -version"**. If your java is installed properly and all environment variables are configured correcly it will show the version of Java installed. Information reflected on the command prompt will be like
```sh
C:UsersJbt>java -version
java version "1.6.0_25"
Java(TM) SE Runtime Environment (build 1.6.0_25-b06)
Java HotSpot(TM) Client VM (build 20.0-b11, mixed mode, sharing)
```
If there is any problem while installing or in setting up the environment variables output on the command prompt will be like
```sh
'java' is not recognized as an internal or external command,
operable program or batch file.
```

#### How to Check if Java is up to date
To know if the Java installed on your System is up to date or not [Check here](http://www.java.com/en/download/installed.jsp)

#### First Java Program
It is highly common that the very first Java program would be to print "Hello World!!". 
If everything till now was configured properly then we can start writing our first application. Open any editor and write the bellow code.
```sh
public class FirstProgram {
  public static void main(String args[]) {
    System.out.println("Hello World!");
  }
}
```
Once done save the file with the name "FirstProgram.java". Please note that the name of the file should be the same as the name given to public class. And fire **"javac"** command which is used to compile the java code as below
```sh
C:java-core>javac FirstProgra.java
```
If the java file is complied properly the compiler will create a class file for the java source file.

#### How to Run Java Application
Now that your java file is compiled we can execute the application with the help of **"java"** command as beflow
