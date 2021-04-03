# Java BigInteger

## In this problem, you have to add and multiply huge numbers! These numbers are so big that you can't contain them in any ordinary data types like a long integer. Use the power of Java's BigInteger class and solve this problem.

```
Sample Input

1234
20
```

```
Sample Output

1254
24680
```

```
import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        BigInteger Num1, Num2, AddNum1Num2, MulNum1Num2;
        Num1 = new BigInteger(input.next());
        Num2 = new BigInteger(input.next());
        System.out.println(Num1.add(Num2));
        System.out.println(Num1.multiply(Num2));
        
    }
}

```

```
OUTPUT:

1254
24680
```
