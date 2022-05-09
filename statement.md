# Welcome!

This Java template lets you get started quickly with a simple one-page playground.

```java runnable
// { autofold
import java.util.*;

public class Main {

    // Returns the distance between the two closest numbers.
    static int distClosestNumbers(int[] numbers) {
        Arrays.sort(numbers);
        int dist = numbers[0];
        for (int i = 1; i < numbers.length; i++) {
            if ((numbers[i] - numbers[i-1]) < dist) {
            dist = numbers[i] - numbers[i-1];
            }
        }
        return dist;
        // try to implement it!
    }
   
    public static void main(String[] args) {
        int[] testArray = {3, 9, 50, 15, 99, 7, 98, 65};
        int result = distClosestNumbers(testArray);
        System.out.println(result); // Expected result is 1 (the 2 closest numbers are 98 and 99)
    }
}
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced Java template](https://tech.io/select-repo/385)
