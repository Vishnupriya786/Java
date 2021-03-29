# Java Loops I

```
Task
Given an integer,N , print its first 10 multiples. Each multiple Nxi (where 1<=i<=10) should be printed on a new line in the form: N x i = result.
```

```
Sample Input

2
```

```
Sample Output

2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20
```

```
import java.util.*;
class Solution{
    public static void main(String a[]){
        Scanner input = new Scanner(System.in);
        int Number = input.nextInt();
        for (int num = 1; num<=10; num++){
            int Result = Number * num;
            System.out.println(Number+" x "+num+" = "+Result);
        }
    }
}
```

```
OUTPUT:

2 x 1 = 2
2 x 2 = 4
2 x 3 = 6
2 x 4 = 8
2 x 5 = 10
2 x 6 = 12
2 x 7 = 14
2 x 8 = 16
2 x 9 = 18
2 x 10 = 20
```
