# Ex15 Value Existence Check in a TreeMap
## Date: 12.2.26
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1.Read all key–value pairs and store them inside a TreeMap.

2.Take the value to be searched as input.

3.Use containsValue() to check if the TreeMap has that value.

4.If it exists, print a success message.

5.Otherwise, print that the value does not exist.  

## Program:
```
/*
Program to checks whether a given value exists in a TreeMap.
Developed by: Sri Yaline R
RegisterNumber: 212224040325
```
```
import java.util.*;

public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if(map.containsValue(searchValue)){
            System.out.println("Value \""+searchValue + "\" exists in the TreeMap.");
        }
        else{
             System.out.println("Value \""+searchValue + "\" does not exist in the TreeMap.");
            
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}

*/
```

## Output:
<img width="1148" height="733" alt="image" src="https://github.com/user-attachments/assets/f41153c5-3f58-4684-8243-7460dd2a6016" />



## Result:
Thus, JAVA program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
