# Ex11 Convert HashSet to ArrayList in Java
## Date: 8.2.26
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1.Create an empty ArrayList.

2.Traverse each element in the HashSet.

3.Add each element to the ArrayList.

4.After the loop, the ArrayList contains all set elements.

5.Return the ArrayList as the final result.

## Program:
```
/*
Program to To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
Developed by: Sri Yaline R
RegisterNumber: 212224040325
```
```
import java.util.*;

public class HashSetToArrayList {

    public static ArrayList<Integer> convertToArrayList(HashSet<Integer> set) {
      ArrayList<Integer> list=new ArrayList<>();
      for (Integer num : set){
          list.add(num);
      }
      return list;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        HashSet<Integer> set = new HashSet<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            set.add(num);
        }

        ArrayList<Integer> list = convertToArrayList(set);
        System.out.println("ArrayList contents:");
        for (int num : list) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

*/
```

## Output:
<img width="759" height="639" alt="image" src="https://github.com/user-attachments/assets/873e96bd-193f-422b-9d33-bc6367819bc8" />



## Result:
The JAVA program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
