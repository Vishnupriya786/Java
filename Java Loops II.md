# Java Loops II

```
We use the integers a, b, and n to create the following series:

(a+2^0.b), (a+2^0.b+2^1.b),....(a+2^0.b+2^1.b+.....+2^(n-1).b)

You are given q queries in the form of a, b, and n. For each query, print the series corresponding to the given a, b, and n values as a single line of n space-separated integers.
```

```
Sample Input

2
0 2 10
5 3 5
```

```
Sample Output

2 6 14 30 62 126 254 510 1022 2046
8 14 26 50 98
```

```
import java.util.*;
import java.io.*;
import java.math.*;
class Solution{
    
    public static void main(String []argh){
        Scanner in = new Scanner(System.in);
        int t=in.nextInt();
        for(int i=0;i<t;i++){
            int a = in.nextInt();
            int b = in.nextInt();
            int n = in.nextInt();
            double sum = a+(Math.pow(2,0)*b);
            for (int num = 1; num<=n; num++){
                System.out.print((int)sum+" ");
                sum += (Math.pow(2,num))*b;
                
            }
            System.out.println();
        }
    }
}
```

```
OUTPUT:

2 6 14 30 62 126 254 510 1022 2046
8 14 26 50 98
```
