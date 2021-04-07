# Java Substring

## Given a string, s, and two indices, start and end, print a substring consisting of all characters in the inclusive range from start to end-1. You'll find the String class' substring method helpful in completing this challenge.

```
Sample Input

Helloworld
3 7
```

```
Sample Output

lowo
```

```
import java.util.*;
class Solution{
    public static void main(String arr[]){
        Scanner input = new Scanner(System.in);
        String Word = input.next();
        int StartIndex = input.nextInt();
        int EndIndex = input.nextInt();
        System.out.println(Word.substring(StartIndex, EndIndex));
    }
}

```

```
OUTPUT:

lowo
```
