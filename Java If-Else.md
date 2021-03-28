# Java If-Else

```
Given an integer, n, perform the following conditional actions:

If n is odd, print Weird
If n is even and in the inclusive range of 2 to 5, print Not Weird
If n is even and in the inclusive range of 6 to 20, print Weird
If n is even and greater than 20, print Not Weird
```

```
Sample Input 0

3
```

```
Sample Output 0

Weird
```

```
import java.util.*;
class Solution{
    public static void main(String a[]){
        Scanner input = new Scanner(System.in);
        int Number1 = input.nextInt();
        if (Number1%2!=0){
            System.out.println("Weird");
        }
        else if(Number1%2==0 && (2<=Number1 && Number1<=5)){
          System.out.println("Not Weird");  
        }
        else if(Number1%2==0 && (6<=Number1 && Number1<=20)){
          System.out.println("Weird");  
        }
        else if(Number1%2==0 && Number1>20){
          System.out.println("Not Weird");  
        }
    }
}
```

```
OUTPUT:

Weird
```
