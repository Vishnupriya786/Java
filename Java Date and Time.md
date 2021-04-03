# Java Date and Time

## The Calendar class is an abstract class that provides methods for converting between a specific instant in time and a set of calendar fields such as YEAR, MONTH, DAY_OF_MONTH, HOUR, and so on, and for manipulating the calendar fields, such as getting the date of the next week. You are given a date. You just need to write the method, getDay(), which returns the day on that date. To simplify your task, we have provided a portion of the code in the editor.

## Input Format: A single line of input containing the space separated month, day and year, respectively, in MM DD YYYY format.

```
Sample Input

08 05 2015
```

```
Sample Output

WEDNESDAY
```

```
import java.io.*;
import java.math.*;
import java.security.*;
import java.text.*;
import java.util.*;
import java.util.concurrent.*;
import java.util.regex.*;
import java.time.*;

class Result {
    public static String findDay(int month, int day, int year) {
        return LocalDate.of(year,month,day).getDayOfWeek().name(); 
    }
}
```

```
OUTPUT:

WEDNESDAY
```
