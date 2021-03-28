# Java Stdin and Stdout II

```
In this challenge, you must read an integer, a double, and a String from stdin, then print the values according to the instructions in the Output Format section below. To make the problem a little easier, a portion of the code is provided for you in the editor.
```

```
Input Format

There are three lines of input:

The first line contains an integer.
The second line contains a double.
The third line contains a String.
```

```
Output Format

There are three lines of output:

On the first line, print String: followed by the unaltered String read from stdin.
On the second line, print Double: followed by the unaltered double read from stdin.
On the third line, print Int: followed by the unaltered integer read from stdin.
```

```
Sample Input

42
3.1415
Welcome to HackerRank's Java tutorials!
```

```
Sample Output

String: Welcome to HackerRank's Java tutorials!
Double: 3.1415
Int: 42
```

```
import java.util.*;
class Solution{
    public static void main(String a[]){
        Scanner input = new Scanner(System.in);
        int Number1 = input.nextInt();
        double Number2 = input.nextDouble();
        String Word = input.nextLine();
        Word = input.nextLine();
        System.out.println("String: "+Word);
        System.out.println("Double: "+Number2);
        System.out.println("Int: "+Number1);
        
    }
}
```

```
OUTPUT:

String: Welcome to HackerRank's Java tutorials!
Double: 3.1415
Int: 42
```
