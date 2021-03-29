# Java Output Formatting

```
Input Format

Every line of input will contain a String followed by an integer.
Each String will have a maximum of 10 alphabetic characters, and each integer will be in the inclusive range from 0 to 999.

Output Format

In each line of output there should be two columns:
The first column contains the String and is left justified using exactly 15 characters.
The second column contains the integer, expressed in exactly 3 digits; if the original input has less than three digits, you must pad your output's leading digits with zeroes.
```

```
Sample Input

java 100
cpp 65
python 50
```

```
Sample Output

================================
java           100 
cpp            065 
python         050 
================================
```

```
Explanation

Each String is left-justified with trailing whitespace through the first 15 characters. The leading digit of the integer is the 16th character, and each integer that was less than 3 digits now has leading zeroes.
```

```
import java.util.Scanner;

public class Solution {

    public static void main(String[] args) {
            System.out.println("================================");
            Scanner input = new Scanner(System.in);
            for (int Range = 1;Range<=3;Range++){
                 String Word = input.next();
                 int Number = input.nextInt();
                 System.out.printf("%-15s%03d\n",Word,Number);
            }
            System.out.println("================================");
    }
}
```

```
OUTPUT:

================================
java           100 
cpp            065 
python         050 
================================
```
