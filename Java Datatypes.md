# Java Datatypes


Java has 8 primitive data types; char, boolean, byte, short, int, long, float, and double. For this exercise, we'll work with the primitives used to hold integer values (byte, short, int, and long):

A byte is an 8-bit signed integer.
A short is a 16-bit signed integer.
An int is a 32-bit signed integer.
A long is a 64-bit signed integer.
Given an input integer, you must determine which primitive data types are capable of properly storing that input.

To get you started, a portion of the solution is provided for you in the editor.

## Input Format
The first line contains an integer, T, denoting the number of test cases.
Each test case, T, is comprised of a single line with an integer, n, which can be arbitrarily large or small.

## Output Format
For each input variable n and appropriate primitive datatype, you must determine if the given primitives are capable of storing it. If yes, then print:
## n can be fitted in:
## * dataType
if no, print
## n can't be fitted anywhere.

```
Sample Input

5
-150
150000
1500000000
213333333333333333333333333333333333
-100000000000000
```

```
Sample Output

-150 can be fitted in:
* short
* int
* long
150000 can be fitted in:
* int
* long
1500000000 can be fitted in:
* int
* long
213333333333333333333333333333333333 can't be fitted anywhere.
-100000000000000 can be fitted in:
* long
```

```
import java.util.*;
import java.io.*;
class Solution{
    public static void main(String []argh)
    {
        Scanner sc = new Scanner(System.in);
        int t=sc.nextInt();
        for(int i=0;i<t;i++)
        {
            try
            { 
                long min = -9223372036854775808L;
                long max = 9223372036854775807L;
                long x=sc.nextLong();
                System.out.println(x+" can be fitted in:");
                if(x>=-128 && x<=127)System.out.println("* byte");
                if (-32768 <= x && x <= 32767){
                    System.out.println("* short");
                }
                if (-2147483648 <= x && x <= 2147483647){
                    System.out.println("* int");
                }
                if (min <= x && x <= max){
                    System.out.println("* long");
                }
            }
            catch(Exception e)
            {
                System.out.println(sc.next()+" can't be fitted anywhere.");
            }

        }
    }
}

```

```
OUTPUT:

-150 can be fitted in:
* short
* int
* long
150000 can be fitted in:
* int
* long
1500000000 can be fitted in:
* int
* long
213333333333333333333333333333333333 can't be fitted anywhere.
-100000000000000 can be fitted in:
* long
```
