Here's a sample Java code to find Armstrong number:


```java
import java.util.Scanner;


public class ArmstrongNumber {



```
public static void main(String[] args) {

    int num, temp, remainder, sum = 0, n = 0;

    Scanner scanner = new Scanner(System.in);
    System.out.println("Enter a number:");

    num = scanner.nextInt();
    temp = num;

    // Count number of digits
    while (temp != 0) {
        n++;
        temp /= 10;
    }

    temp = num;

    while (temp != 0) {
        remainder = temp % 10;
        sum += Math.pow(remainder, n);
        temp /= 10;
    }

    if (num == sum) {
        System.out.println(num + " is an Armstrong number.");
    } else {
        System.out.println(num + " is not an Armstrong number.");
    }
}

```

}
```


In this code, we are using a Scanner to read input from the user. Then we are finding the number of digits in the input number. We are extracting each digit from the number and computing the sum of the digits raised to the power of the number of digits. If the computed sum equals the input number, then it is an Armstrong number. Otherwise, it is not an Armstrong number.

