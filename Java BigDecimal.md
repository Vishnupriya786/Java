# Java BigDecimal

## Given an array, s, of n real number strings, sort them in descending order.

```
Sample Input

9
-100
50
0
56.6
90
0.12
.12
02.34
000.000
```

```
Sample Output

90
56.6
50
02.34
0.12
.12
0
000.000
-100
```

```

import java.util.*;
class Solution{

    public static void main(String []args){
        //Input
        Scanner sc= new Scanner(System.in);
        int n=sc.nextInt();
        String []s=new String[n+2];
        for(int i=0;i<n;i++){
            s[i]=sc.next();
        }
      	sc.close();
        Comparator<String> CompareBigDecimal = new Comparator<String>(){
            public int compare(String a,String b){
                BigDecimal num1 = new BigDecimal(a);
                BigDecimal num2 = new BigDecimal(b);
                return num2.compareTo(num1);
            }
        };
        Arrays.sort(s,0,n,CompareBigDecimal);

        //Output
        for(int i=0;i<n;i++)
        {
            System.out.println(s[i]);
        }
    }

}
```

```
OUTPUT:

90
56.6
50
02.34
0.12
.12
0
000.000
-100
```
