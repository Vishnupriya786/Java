# Java Strings Introduction

## This exercise is to test your understanding of Java Strings. A sample String declaration:
## String myString = "Hello World!"
## The elements of a String are called characters. The number of characters in a String is called the length, and it can be retrieved with the String.length() method. Given two strings of lowercase English letters, a and b, perform the following operations:
## Sum the lengths of A and B.
## Determine if A is lexicographically larger than B (i.e.: does B come before A in the dictionary?).
## Capitalize the first letter in A and B and print them on a single line, separated by a space.

```
Sample Input 0

hello
java
```

```
Sample Output 0

9
No
Hello Java
```

```
import java.util.*;
class Solution{
    public static void main(String arr[]){
        Scanner input = new Scanner(System.in);
        String Word1 = input.next();
        String Word2 = input.next();
        System.out.println(Word1.length()+Word2.length());
        ArrayList lis = new ArrayList();
        lis.add(Word1);
        lis.add(Word2);
        Collections.sort(lis);
        if (lis.get(0)== Word1){
            System.out.println("No");
        }
        else{
            System.out.println("Yes");
        }
        String FirstLetterWord1 = Word1.substring(0, 1);
        String RemainingLetterWord1 = Word1.substring(1, Word1.length());
        
        FirstLetterWord1 = FirstLetterWord1.toUpperCase();
        System.out.print(FirstLetterWord1 + RemainingLetterWord1+" ");
        
        String FirstLetterWord2 = Word2.substring(0, 1);
        String RemainingLetterWord2 = Word2.substring(1, Word2.length());
        
        FirstLetterWord2 = FirstLetterWord2.toUpperCase();
        System.out.println(FirstLetterWord2 + RemainingLetterWord2);
    }
}

```

```
OUTPUT

9
No
Hello Java
```
