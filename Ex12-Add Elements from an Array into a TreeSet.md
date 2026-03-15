
# Ex12 Add Elements from an Array into a TreeSet
## Date: 9.2.26
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1.Create an empty TreeSet.

2.Traverse each element of the array.

3.Insert every element into the TreeSet.

4.TreeSet automatically removes duplicates and sorts the elements.

5.Return the TreeSet for printing or further use.

## Program:
```
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: Sri Yaline R
RegisterNumber: 212224040325
```
```
import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        TreeSet<Integer> ts=new TreeSet<>();
        for(int i:arr){
            ts.add(i);
        }
        return ts;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}

*/
```

## Output:
<img width="939" height="522" alt="image" src="https://github.com/user-attachments/assets/c3d5758e-dc7c-4c66-8400-7884931020b5" />




## Result:
The JAVA program successfully adds elements from an array into a TreeSet.
