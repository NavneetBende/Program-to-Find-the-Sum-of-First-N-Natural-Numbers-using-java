# Program-to-Find-the-Sum-of-First-N-Natural-Numbers-using-java


Find the Sum of First N Natural Numbers in Java
Find the Sum of First N Natural Numbers in Java
Given an integer input the objective is to write a code to Find the Sum of N Natural Numbers in C++. To do so we simply keep adding the value of the iter variable using a for loop.

Example
Input : num = 5
Output : 15

Where first 8 number is 1, 2, 3, 4, 5
Sum of numbers = 1 + 2 + 3 + 4 + 5 = 15
Find the Sum of First N Natural Numbers in Java
Given an integer input of N, the objective is to find the sum of all the natural numbers until the given input integer. To do so we can use different approaches to write the Java code and some such methods are mentioned below,

Method 1: Using for Loop
Method 2: Using Formula for the Sum of Nth Term
Method 3: Using Recursion
We’ll discuss and learn more about each above-mentioned method in detail in the sections below.

Related Pages
Sum of N natural numbers

Sum of numbers in a given range

Greatest of two numbers

Greatest of the Three numbers

Leap year or not

Method 1 : Using for Loop
In this method we’ll add all the natural numbers until the given integer input using for loop in Java.

Java Code
public class Main
 {
   public static void main (String[]args)
   {

     int n = 10;
     int sum = 0;

     for (int i = 1; i <= n; i++)
         sum += i;
       System.out.println (sum);
   }
 }
Output
55
Explanation
Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

In the main() function initialize the required variables.
Run a for loop with range as N+1.
Keep adding the iter values to the Sum variable.
Print Sum variable.
The output for the above mentioned code is the sum of all the natural numbers until the given value.

Method 2 : Using Formula for the Sum of Nth Term
In this Method we use the formula for finding the sum of N term.

Formula to Find the Sum of N terms
Sum = ( Num * ( Num + 1 ) ) / 2
Java Code
public class Main
 {
   public static void main (String[]args)
   {

     int n = 10;

       System.out.println ( n*(n+1)/2);
   }
 }
Output
55
Explanation
Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

In the main() function initialize the required variables.
Substitute n with num variable in the above code and store it in sum variable.
Print Sum variable.
This algorithm uses the formula n(n+1)/2 that can be used to find sum of first N natural numbers. This also reduces the time complexity from O(n) to O(1). The output for the above mentioned code is the sum of all the natural numbers until the given value.

Method 3 : Using Recursion
This method uses Recursion to recursively add the natural numbers up to the given integer input using Recursion in Java.

Java Code
public class Main
{
  public static void main (String[]args)
  {

    int n = 10;
    int sum = getSum (n);

      System.out.println (sum);
  }

  static int getSum (int n)
  {
    if (n == 0)
      return n;

    return n + getSum (n - 1);
  }
}
Output
55
Explanation
Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we recursively call a function  iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

Define a Recursive function getSum() which takes the number input as an argument.
Recursively call the function and keep on adding the return statements.
In the main() function initialize the required variables.
Call the Recursive function and print out the returned value.
The output for the above mentioned code is the sum of all the natural numbers until the given value.
