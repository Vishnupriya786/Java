# Java Stdin and Stdout I

```
In this challenge, you must read 3 integers from stdin and then print them to stdout. Each integer must be printed on a new line. To make the problem a little easier, a portion of the code is provided for you in the editor below.
```

```
Sample Input

42
100
125
```

```
Sample Output

42
100
125
```

```
import java.util.*;
class Solution{
    public static void main(String a[]){
        Scanner input = new Scanner(System.in);
        int Number1 = input.nextInt();
        int Number2 = input.nextInt();
        int Number3 = input.nextInt();
        System.out.println(Number1);
        System.out.println(Number2);
        System.out.println(Number3);
    }
}
```

```
OUTPUT:

42
100
125
```
