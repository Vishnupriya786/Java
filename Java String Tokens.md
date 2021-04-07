# Java String Tokens

## Given a string, s, matching the regular expression [A-Za-z !,?._'@]+, split the string into tokens. We define a token to be one or more consecutive English alphabetic letters. Then, print the number of tokens, followed by each token on a new line.

## Note: You may find the String.split method helpful in completing this challenge.

```
Sample Input

He is a very very good boy, isn't he?
```

```
Sample Output

10
He
is
a
very
very
good
boy
isn
t
he
```

```
import java.util.*;
class Solution{
    public static void main(String arr[]){
        Scanner input = new Scanner(System.in);
        String word = input.nextLine() ;
        word = word.trim();
        if(word.length()==0){
            System.out.println(0);
            return;
        }
        
        String array[] = word.trim().split("[ !,?.\\_'@]+");
        System.out.println(array.length);
        for(String words : array) {
            System.out.println(words);
        }
        
        
    }
}

```

```
OUTPUT:
10
He
is
a
very
very
good
boy
isn
t
he
```
