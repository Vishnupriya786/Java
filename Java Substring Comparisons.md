# Java Substring Comparisons

## We define the following terms:

## Lexicographical Order, also known as alphabetic or dictionary order, orders characters as follows:    A<Z<a<z
## For example, ball < cat, dog < dorm, Happy < happy, Zoo < ball.

## A substring of a string is a contiguous block of characters in the string. For example, the substrings of abc are a, b, c, ab, bc, and abc.
## Given a string, s, and an integer, k, complete the function so that it finds the lexicographically smallest and largest substrings of length k.

```
Sample Input 0

welcometojava
3
```

```
Sample Output 0

ava
wel
```

```
import java.util.Scanner;

public class Solution {

    public static String getSmallestAndLargest(String s, int k) {
        java.util.ArrayList lis = new java.util.ArrayList();
        for (int i=0;i<=s.length()-k;i++){
            lis.add(s.substring(i,i+k));
        }
        java.util.Collections.sort(lis);
        return (lis.get(0))+"\n"+ (lis.get(lis.size()-1));
        
    }


    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        String s = scan.next();
        int k = scan.nextInt();
        scan.close();
      
        System.out.println(getSmallestAndLargest(s, k));
    }
}
```

```
OUTPUT:

ava
wel
```
