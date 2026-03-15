# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## Date: 10.2.26
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1.Create a new array of the given size.

2.Use Arrays.fill() to assign the same value to all positions.

3.This fills every index with the given constant value.

4.Return the filled array.

5.Print the array elements in the main method.

  

## Program:
```
/*
Program to FILL the first 10 elements of an array with a constant value using the Arrays.fill() method.
Developed by: Sri Yaline R
RegisterNumber: 212224040325
```
```
import java.util.*;

public class FillArrayUsingArraysFill {

    public static int[] fillArray(int size, int value) {
       int a[]=new int[size];
       Arrays.fill(a,value);
       return a;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}
  
*/
```

## Output:

<img width="836" height="302" alt="image" src="https://github.com/user-attachments/assets/aa85540e-454a-4492-be92-eca8364fc63c" />


## Result:
The JAVA program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
