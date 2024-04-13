Program to reverse the string
In this article we will learn how to reverse a string in Java

Reversing a string is a technique so that the 1st character becomes the last character and so on.

Suppose we have a string called “prepinsta” so we have to find reverse of that string is “atsniperp” we can do this in two way by using reverse method of StringBuilder class and by using normal for loop with charAt() method.

reverse a string
Algorithm
Take a string input from the user
Store it in the variable called “s” in this case
After that we will append that string variable in the StringBuilder
After that reverse the StringBuilder object by using  the reverse function.
program to reverse a string
Code in Java (Program to reverse the string)
Run
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
    String s ="Prepinsta";
    StringBuilder sb = new StringBuilder();
    sb.append(s);
    System.out.println( "String is : "+sb);
    sb.reverse();
   System.out.println("Reversed string is : "+sb);
  }
}
String is : Prepinsta
Reversed string is : atsniperP
(Method-2)
Take a string input from the user
Store it in the variable called “s” in this case
Take a String “rev” variable and initialize with empty string
Start i for loop start from i=s.length()-1 to i>=0
Get one by one character with the help of charAt() and store it in the “rev” variable 
At last print that “rev” variable
Code In Java
Run
import java.util.Scanner;
public class Main {
  public static void main(String[] args) {
    String s = "prepinsta";
    String rev = "";

    for (int i = s.length()-1; i >=0; i--) {
      rev=rev+s.charAt(i);
    }
    System.out.println(rev);
  }
}
Output
String is : prepinsta
Reversed string is : atsniperp
