# Java Anagrams

## Two strings, a and b, are called anagrams if they contain all the same characters in the same frequencies. For this challenge, the test is not case-sensitive. For example, the anagrams of CAT are CAT, ACT, tac, TCA, aTC, and CtA.

```
Sample Input 0

anagram
margana
```

```
Sample Output 0

Anagrams
```

```
import java.util.Scanner;

public class Solution {

    static boolean isAnagram(String a, String b) {
        a = a.toLowerCase();
        b = b.toLowerCase();
        char[] aw = a.toCharArray();
        char[] bw = b.toCharArray();
        java.util.Arrays.sort(aw);
        java.util.Arrays.sort(bw);
        
        if (java.util.Arrays.equals(aw, bw)) {
            return true;
        }
        else{
            return false;
        }
    }

    public static void main(String[] args) {
    
        Scanner scan = new Scanner(System.in);
        String a = scan.next();
        String b = scan.next();
        scan.close();
        boolean ret = isAnagram(a, b);
        System.out.println( (ret) ? "Anagrams" : "Not Anagrams" );
    }
}
```

```
OUTPUT:
Anagrams
```
